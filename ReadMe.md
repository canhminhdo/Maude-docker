# Maude Docker Image

This repository contains a docker image for Maude and some Maude code examples.

### Prerequisites
- We have installed the latest version of [Docker Desktop](https://docs.docker.com/get-docker/)
- We have installed a [Git client](https://git-scm.com/downloads)
- We have an IDE or a text editor to edit files. We recommend using [Visual Studio Code](https://code.visualstudio.com/)
- Get used to using Terminal. We recommend studying (UNIX tutorial for beginners)[http://www.ee.surrey.ac.uk/Teaching/Unix/].

### How To Use

1. Clone this repository using the following command:

`git clone https://github.com/canhminhdo/Maude-docker.git`


2. Running a docker container in an interacting mode using the following command:

`docker compose run --rm code`

We use running service `code` with the argument `--rm` for removing the container after use.

3. Running an example with Maude in the container using the following commands:

- Firstly, we need to start up the Maude application using the following command:

`maude`

- Secondly, we may want to load the specification of an example into Maude. 

For example, we load examples/Qlock.maude file into Maude using the following command.

`in examples/qlock.maude`

- Lastly, we can conduct a model-checking experiment for Qlock using the following command:

`red in QLOCK-CHECK : modelCheck(init,lofree) .`

4. Using a text editor to compose a maude file.

Open the folder containing this cloned repository using a text editor, namely Visual Code Studio.

We need to save Maude files into this folder to make them available to the container.

Once we complete composing a Maude file, we can feed it to Maude in the contain as instructed in Step 3.

### Questions
If you have any questions, please ask me at [here](mailto:canhdo@jaist.ac.jp).