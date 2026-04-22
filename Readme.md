# Foundry Local workshop (Python)

Fooundry Local is quick experimentation and production platform for hardware optimized language model inferencing on device (on edge).<br>
This workshop provides step-by-step Foundry Local learning with a few lines of code and background explanation for beginners.

1. [Getting started](./01_get_started.ipynb)
2. [Run as web service (Integration)](./02_run_as_web_service.ipynb)
3. [Integrate with Agent Framework](./03_agent_framework.ipynb)
4. Transcribe audio (coming soon ...)
5. Bring your own (BYO) models  (coming soon ...)

All contents in this repository are experimented on Azure virtual machine with a single NVIDIA Tesla T4 GPU (NC4as T4 v3).

> Note : Foundry Local is for **single user**. For multiple users, use other platforms - vLLM, Triton Inference Server, etc. (Foundry Local doesn't provide features optimized for multiple users - such as, continuous batching, paged attention, ...)

## Prerequisites

The installation is pretty simple.<br>
Just install **Foundry Local SDK** for Python as follows. (This command will also install and setup ONNX runtime core and Foundry core.)

<ins>For Windows</ins>

```
pip install foundry-local-sdk-winml openai
```

<ins>For cross-platform (MacOS / Linux)</ins>

```
pip install foundry-local-sdk openai
```

For running Lesson 3, also install Agent Framework package as follows.

```
pip install agent-framework
```

For running Lesson 5, also install Olive package (which can convert models to ONNX format) as follows.

```
pip install olive-ai[auto-opt]
```

Finally, clone this repository in your working environment as follows.

```
git clone https://github.com/tsmatsuz/foundry-local-tutorials
cd foundry-local-tutorials
```

> Note : You can also manage with **Foundry Local CLI**, which runs on top of SDK. Now Foundry Local CLI for Linux is, however, under construction.

## Official document

The purpose of this repository is to learn with code and clear explanation (background) for beginners in each step.<br>
In [official document](https://learn.microsoft.com/en-us/azure/foundry-local/), you can find tutorials and how-to guides for Foundry Local.

*Tsuyoshi Matsuzaki @ Microsoft Asia*
