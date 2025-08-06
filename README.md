# KB Assistant Challenge

## Objective

Your task is to build a system that enables users to query contextual information from the script of the movie The Matrix. The system should retrieve relevant excerpts from the script and use them to help an AI agent generate accurate, context-aware responses.

You may use a Retrieval-Augmented Generation (RAG) approach, or any alternative design that effectively combines retrieval and generation to produce grounded answers. The focus is on building a solution that demonstrates strong retrieval capabilities and uses that context effectively in AI-driven responses.

## Challenge Goals

This challenge is divided into two parts:

-   Part 1 (Mandatory): Completing this part is required for your submission to be considered complete.
-   Part 2 (Optional but Recommended): This part is not required but will demonstrate deeper reasoning, richer retrieval, and more advanced capabilities.

### Part 1 - Core Functionality (Mandatory)

Your system must be able to answer basic factual queries based on the provided script of **The Matrix**.

Example queries:

-   Under what circumstances does Neo see a white rabbit?
-   How did Trinity and Neo first meet?
-   Why is there no sunlight in the future?
-   Who needs solar power to survive?
-   Why do the Agents want to capture Morpheus?
-   Describe the Nebuchadnezzar
-   What is Nebuchadnezzar's crew made up of?

### Part 2 - Advanced Capabilities (Optional)

This part evaluates your system's ability to handle complex, composed, and reasoning-based queries.

Example queries:

-   How many times does Morpheus mention that Neo is the One?
-   Why are humans similar to a virus? And who says that?
-   Describe Cypher's personality.
-   What does Cypher offer to the Agents, and in exchange for what?
-   What is the purpose of the human fields, and who created them?

## Enviroment setup

_This setup is highly recommended but not obligatory. Work on the challenge using the environment of your preference._

### Prerequisites

-   Install Make:

    ```bash
    sudo apt install make
    ```

-   Install Docker following the official [Docker installation guide](https://docs.docker.com/engine/install/ubuntu/).

### Dev container (Recommended)

To ensure a consistent development environment, this project uses a preconfigured Dev Container.

-   Open this repository in VS Code:
    ```bash
    code .
    ```
-   After installing the [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension, press F1 and type _Dev Containers_ and select: **Reopen in Container**

### Jupyter

Jupyter is preconfigured inside the Dev Container.
You can explore examples in the [notebooks/](notebooks/) directory.
When opening a notebook, select the appropriate kernel in the top-right corner: **Python Environments -> Python 3.12 (Global Env)**

### Custom python lib

A local Python package named **kbac** (short for KB Assistant Challenge) is included in the environment. It contains utility functions to help you work with the project. You are encouraged to extend this library as needed. Example usage can be found in: [notebooks/01-loaders/01-matrix-script-loader.ipynb](notebooks/01-loaders/01-matrix-script-loader.ipynb).

### Python requirements

Yo can install additional python libraries adding it to the **requirements.txt**
