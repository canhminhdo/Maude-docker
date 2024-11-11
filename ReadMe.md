# A Docker Image for Maude 3.5

This repository contains a Docker image for Maude 3.5 and some Maude code examples.

### Prerequisites
- The latest version of [Docker Desktop](https://docs.docker.com/get-docker/)
- [A git client](https://git-scm.com/downloads)
- An IDE or a text editor to compose files (e.g., [Visual Studio Code](https://code.visualstudio.com/)).
- Get used to using Terminal (studying [UNIX tutorial for beginners](http://www.ee.surrey.ac.uk/Teaching/Unix/)).

### How To Use

1. Clone this repository using the following command:

    `git clone https://github.com/canhminhdo/Maude-docker.git`


2. Run a Docker container with our pre-built Docker image for Maude 3.5 in interactive mode using the following command:

    `docker compose run --rm code`

    Here, we run the service `code` with the argument `--rm` to automatically remove the container after use.

3. Run an example with Maude in the container using the following commands:

- First, we start the Maude application using the following command:

    `maude`

- Second, we load the specification of an example into Maude. For example, we use Qlock as the example with the following command:

    `in examples/qlock.maude`

- Finally, we can conduct a model-checking experiment to verify the lockout freedom property for Qlock using the following command:

    `red in QLOCK-CHECK : modelCheck(init,lofree) .`

4. Use a text editor to compose a Maude file.

- Open the folder containing this cloned repository using a text editor, namely Visual Code Studio.

- Save Maude files into this folder to make them available to the container.

- Once you complete composing a Maude file, you can load it into Maude in the containter as instructed in Step 3.

### Questions
If you have any questions, please ask me at [here](mailto:canhdo@jaist.ac.jp).