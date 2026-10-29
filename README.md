# cicd-final-project

**Project name:** cicd-final-project

This repository contains the Final Project for the Coursera course **CI/CD Tools and Practices**.

It is a Python Flask **Hit Counter** microservice with a complete CI/CD setup:

- **GitHub Actions** CI workflow (`.github/workflows/workflow.yml`) that lints the code with **flake8** and runs the unit tests with **nose**
- **Tekton** tasks (`.tekton/tasks.yml`): a **cleanup** task and a **nose** task, used in an **OpenShift** pipeline

## Setup

After entering the lab environment you will need to run the `setup.sh` script in the `./bin` folder to install the prerequisite software.

```bash
bash bin/setup.sh
```

Then you must exit the shell and start a new one for the Python virtual environment to be activated.

```bash
exit
```

## Running the tests

```bash
nosetests -v --with-spec --spec-color --with-coverage --cover-package=service
```

## License

Licensed under the Apache License. See [LICENSE](/LICENSE)

## Author

Skills Network

## <h3 align="center"> © IBM Corporation 2023. All rights reserved. <h3/>
