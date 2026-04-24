# Foundry Local workshop (Python)

Foundry Local is quick experimentation and production platform for hardware optimized language model inferencing on device (on edge).<br>
This workshop provides step-by-step Foundry Local learning with a few lines of code and background explanation for beginners.

1. [Getting started](./01_get_started.ipynb)
2. [Run as web service (Integration)](./02_run_as_web_service.ipynb)
3. [Integrate with Agent Framework](./03_agent_framework.ipynb)
4. [Transcribe audio (Speech-to-text)](./04_transcribe_audio.ipynb)
5. [Bring your own (BYO) models](./05_byo_models.ipynb)

> Note : Foundry Local is for **single user**. Use this platform for running your application on a single device. (For exposing to multiple users, use other platforms - vLLM, Triton Inference Server, etc. Foundry Local doesn't provide features optimized for multiple users - such as, continuous batching, paged attention, ...)<br>
> Foundry Local powered by Azure Local brings models and agentic AI to customer-owned distributed infrastructure.

## Prerequisites

All contents in this repository are experimented on Azure virtual machine with a single NVIDIA Tesla T4 GPU (NC4as T4 v3) and CUDA 12.8.1.<br>
You can use your own device and hardware acceleration (such as, ROCM, OpenVINO, Qualcomm, ...).

The installation of Foundry Local is pretty simple.<br>
Just install **Foundry Local SDK** for Python as follows. (This command will also install and setup ONNX runtime core and Foundry core.)

<ins>For Windows</ins>

```
pip install foundry-local-sdk-winml openai
```

> Note : On Windows, you should install/update **[Microsoft Visual C++ Redistributable](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist)**. (When it's already installed, you don't need to do anything.)

<ins>For cross-platform (MacOS / Linux)</ins>

```
pip install foundry-local-sdk openai
```

For running Lesson 3, also install Agent Framework package as follows.

```
pip install agent-framework
```

Finally, clone this repository in your working environment as follows.

```
git clone https://github.com/tsmatsuz/foundry-local-workshop
cd foundry-local-workshop
```

In Lesson 5, we also need additional setup (such as, installing ```onnxruntime-genai``` package, etc), but these are written in Lesson5 notebook.

> Note : You can also use and manage with **Foundry Local CLI**, which runs on top of SDK. (Now Foundry Local CLI for Linux is, however, under construction.)<br>
> In this repository, we don't use Foundry Local CLI.

## Official document

The purpose of this repository is to learn with code and clear explanation (background) for beginners in each step.<br>
In [official document](https://learn.microsoft.com/en-us/azure/foundry-local/), you can find tutorials and how-to guides for Foundry Local.

*Tsuyoshi Matsuzaki @ Microsoft Asia*
