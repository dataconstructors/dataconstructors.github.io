# DataConstructors Website

## Getting Started

These instructions will get you a copy of the project up and running on your
local machine for development and testing purposes. If this is not your goal,
you can edit the files Markdown directly on GitHub, open a PR with the changes,
and the CI/CD pipeline will automatically build and deploy the website, once
the PR is merged.

### Installing with Python

1. Install prerequisites

    The following are the prerequisites to build the website locally:

    - Python 3.9 or higher + `pip`: You can install it from [here](https://www.python.org/downloads/).

2. Create a virtual environment

    ```bash
    python3 -m venv env
    ```

3. Activate the virtual environment

    Make sure to activate the virtual environment before proceeding. If you are using
    `bash`, you can do this by running:

    ```bash
    source env/bin/activate
    ```

    On `fish`, you can do this by running:

    ```bash
    source env/bin/activate.fish
    ```

    On `zsh`, you can do this by running:

    ```bash
    source env/bin/activate
    ```

4. Install the required packages (preferably in the virtual environment) using Poetry:


    ```bash
    pip3 install poetry
    poetry install
    ```


### Building the specs

1. To generate the website in the `site/` directory, run:

    ```bash
    mkdocs build
    ```

2. To serve the website locally, run the following command:

    ```bash
    mkdocs serve
    ```

    Take into account that this web server will automatically reload the website
    when you make changes to the files, and it is not especially fast.

3. Deploy the website

    The website is automatically deployed to GitHub Pages when a PR is merged to
    the `main` branch. If you want to deploy the website manually, you can run:

    ```bash
    mkdocs gh-deploy
    ```

    This command will build the website and push the changes to the `gh-pages`
    branch of the repository.

