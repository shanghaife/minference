<div align="center">
<img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />

# Xorbits Inference: Model Serving Made Easy 🤖

[![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
[![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
[![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
[![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
[![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=x&style=for-the-badge)](https://twitter.com/xorbitsio)

English | [中文介绍](README_zh_CN.md) | [日本語](README_ja_JP.md)
</div>
<br />


Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
potential of cutting-edge AI models.

<div align="center">
<i><a href="https://join.slack.com/t/xorbitsio/shared_invite/zt-1z3zsm9ep-87yI9YZ_B79HLB2ccTq4WA">👉 Join our Slack community!</a></i>
</div>

## 🔥 Hot Topics
### Framework Enhancements
- Auto recover: [#694](https://github.com/xorbitsai/inference/pull/694)
- Function calling API: [#701](https://github.com/xorbitsai/inference/pull/701), here's example: https://github.com/xorbitsai/inference/blob/main/examples/FunctionCall.ipynb
- Support rerank model: [#672](https://github.com/xorbitsai/inference/pull/672)
- Speculative decoding: [#509](https://github.com/xorbitsai/inference/pull/509)
- Incorporate vLLM: [#445](https://github.com/xorbitsai/inference/pull/445)
### New Models
- Built-in support for [phi-2](https://huggingface.co/microsoft/phi-2): [#828](https://github.com/xorbitsai/inference/pull/828)
- Built-in support for [mistral-instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2): [#796](https://github.com/xorbitsai/inference/pull/796)
- Built-in support for [deepseek-llm](https://huggingface.co/deepseek-ai) and [deepseek-coder](https://huggingface.co/deepseek-ai): [#786](https://github.com/xorbitsai/inference/pull/786)
- Built-in support for [Mixtral-8x7B-v0.1](https://huggingface.co/mistralai/Mixtral-8x7B-v0.1): [#782](https://github.com/xorbitsai/inference/pull/782)
- Built-in support for [OpenHermes 2.5](https://huggingface.co/teknium/OpenHermes-2.5-Mistral-7B): [#776](https://github.com/xorbitsai/inference/pull/776)
- Built-in support for [Yi](https://huggingface.co/01-ai): [#629](https://github.com/xorbitsai/inference/pull/629)
- Built-in support for [zephyr-7b-alpha](https://huggingface.co/HuggingFaceH4/zephyr-7b-alpha) and [zephyr-7b-beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta): [#597](https://github.com/xorbitsai/inference/pull/597) 
### Integrations
- [Dify](https://docs.dify.ai/advanced/model-configuration/xinference): an LLMOps platform that enables developers (and even non-developers) to quickly build useful applications based on large language models, ensuring they are visual, operable, and improvable.
- [Chatbox](https://chatboxai.app/): a desktop client for multiple cutting-edge LLM models, available on Windows, Mac and Linux.


## Key Features
🌟 **Model Serving Made Easy**: Simplify the process of serving large language, speech 
recognition, and multimodal models. You can set up and deploy your models
for experimentation and production with a single command.

⚡️ **State-of-the-Art Models**: Experiment with cutting-edge built-in models using a single 
command. Inference provides access to state-of-the-art open-source models!

🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources with
[ggml](https://github.com/ggerganov/ggml). Xorbits Inference intelligently utilizes heterogeneous
hardware, including GPUs and CPUs, to accelerate your model inference tasks.

⚙️ **Flexible API and Interfaces**: Offer multiple interfaces for interacting
with your models, supporting OpenAI compatible RESTful API (including Function Calling API), RPC, CLI 
and WebUI for seamless model management and interaction.

🌐 **Distributed Deployment**: Excel in distributed deployment scenarios, 
allowing the seamless distribution of model inference across multiple devices or machines.

🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
with popular third-party libraries including [LangChain](https://python.langchain.com/docs/integrations/providers/xinference), [LlamaIndex](https://gpt-index.readthedocs.io/en/stable/examples/llm/XinferenceLocalDeployment.html#i-run-pip-install-xinference-all-in-a-terminal-window), [Dify](https://docs.dify.ai/advanced/model-configuration/xinference), and [Chatbox](https://chatboxai.app/).

## Why Xinference
| Feature | Xinference | FastChat | OpenLLM | RayLLM |
|---------|------------|----------|---------|--------|
| OpenAI-Compatible RESTful API | ✅ | ✅ | ✅ | ✅ |
| vLLM Integrations | ✅ | ✅ | ✅ | ✅ |
| More Inference Engines (GGML, TensorRT) | ✅ | ❌ | ✅ | ✅ |
| More Platforms (CPU, Metal) | ✅ | ✅ | ❌ | ❌ |
| Multi-node Cluster Deployment | ✅ | ❌ | ❌ | ✅ |
| Image Models (Text-to-Image) | ✅ | ✅ | ❌ | ❌ |
| Text Embedding Models | ✅ | ❌ | ❌ | ❌ |
| More OpenAI Functionalities (Function Calling) | ✅ | ❌ | ❌ | ❌ |

## Getting Started

**Please give us a star before you begin, and you'll receive instant notifications for every new release on GitHub!**

* [Docs](https://inference.readthedocs.io/en/latest/index.html)
* [Built-in Models](https://inference.readthedocs.io/en/latest/models/builtin/index.html)
* [Custom Models](https://inference.readthedocs.io/en/latest/models/custom.html)
* [Deployment Docs](https://inference.readthedocs.io/en/latest/getting_started/using_xinference.html)
* [Examples and Tutorials](https://inference.readthedocs.io/en/latest/examples/index.html)

### Quick Start

Install Xinference by using pip as follows. (For more options, see [Installation page](https://inference.readthedocs.io/en/latest/getting_started/installation.html).)

```bash
pip install "xinference[all]"
```

To start a local instance of Xinference, run the following command:

```bash
$ xinference-local
```

Once Xinference is running, there are multiple ways you can try it: via the web UI, via cURL,
 via the command line, or via the Xinference’s python client. Check out our [docs]( https://inference.readthedocs.io/en/latest/getting_started/using_xinference.html#run-xinference-locally) for the guide.

![web UI](assets/screenshot.png)

## Getting involved

| Platform                                                                                      | Purpose                                            |
|-----------------------------------------------------------------------------------------------|----------------------------------------------------|
| [Github Issues](https://github.com/xorbitsai/inference/issues)                                | Reporting bugs and filing feature requests.        |
| [Slack](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) | Collaborating with other Xorbits users.            |
| [Twitter](https://twitter.com/xorbitsio)                                                      | Staying up-to-date on new features.                |
