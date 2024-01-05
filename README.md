# Guide to Orchestrating Large Language Models (LLMs) <img src="./utils/images/azure_logo.png" alt="Azure Logo" style="width:30px;height:30px;"/>

> This is an early preview and will undergo modifications and changes until the open-source release at the end of February.

This repository provides comprehensive guidance on building end-to-end AI applications using Large Language Models (LLMs) and other Azure AI technologies. It covers various orchestration strategies, offering a roadmap from the initial setup to the deployment of sophisticated LLM applications in the Azure environment.

## Orchestrators to Build Large Language Models (LLMs)

LLMs like Azure's AI services, are versatile for tasks including translation, summarization, and question answering. However, their complexity demands a fine balance of resources and tools. Starting from scratch can lead to extra overhead and technical debt. To mitigate this, LLM Orchestrators have emerged, simplifying application building and integrating into AI application layers for accelerated development.

#### 🔄 Comparing LLM Orchestration Frameworks 

- **Prompt Flow** is a low-level orchestration tool, ideal for creating and debugging AI flows, especially for interactions with LLMs. Being a low-level tool, it provides more control and flexibility to developers. It allows developers to directly manipulate the underlying systems and processes. However, it may require more time and expertise to use effectively.

- **Langchain** and **Semantic Kernel** are high-level frameworks. They excel in complex applications, offering more out-of-the-box tools and integrations, primarily in Python and JavaScript (Langchain) and C# and Python (Semantic Kernel). High-level frameworks abstract away many of the complexities of the underlying systems, making them easier to use for developers. They provide built-in functionalities and are generally more user-friendly. However, they may offer less flexibility and control compared to low-level tools.

### Prompt Flow: A Low-Level Orchestration Tool
Prompt Flow is an essential suite of tools for LLM-based AI application development. It aids in creating, developing, and evaluating AI applications, providing a streamlined path from concept to production. As a low-level tool, it requires a deeper understanding of the underlying systems but offers more control and customization options.

### Langchain and Semantic Kernel: High-Level Frameworks
Langchain and Semantic Kernel are two standout high-level LLM frameworks, each with unique features and use cases. They abstract away many of the complexities of the underlying systems, providing a more user-friendly interface. They come with a variety of built-in tools and integrations, making them ideal for complex applications. However, they may not offer as much flexibility for custom plugin chaining as low-level tools like Prompt Flow.

## 💼 Contributing
+ Want to contribute? Check our **[CONTRIBUTING](./CONTRIBUTING.md)** guide!
- For latest updates and significant changes, see [CHANGELOG.md](CHANGELOG.md).

## 🌲 Project Tree Structure

```
📂 gbbai-llmops-orchestrators
┣ 📂 notebooks <- For development, EDA, and quick testing (Jupyter notebooks for analysis and development). README
┣ 📂 orchestrators <- Sample projects using the three orchestrators mentioned above.
┣ 📦 src <- Houses main source code.
┣ 📂 test <- Runs unit and integration tests for code validation and QA. Check README.
┣ 📂 utils <- Contains utility functions and shared code used throughout the project. Detailed info in README
┣ 📜 .pre-commit-config.yaml <- Config for pre-commit hooks ensuring code quality and consistency.
┣ 📜 CHANGELOG.md <- Logs project changes, updates, and version history.
┣ 📜 CONTRIBUTING.md <- Guidelines for contributing to the project.
┣ 📜 environment.yaml <- Conda environment configuration.
┣ 📜 Makefile <- Simplifies common development tasks and commands.
┣ 📜 pyproject.toml <- Configuration file for build system requirements and packaging-related metadata.
┣ 📜 README.md <- Overview, setup instructions, and usage details of the project.
┣ 📜 requirements-codequality.txt <- Requirements for code quality tools and libraries.
┣ 📜 requirements.txt <- General project dependencies.
```
