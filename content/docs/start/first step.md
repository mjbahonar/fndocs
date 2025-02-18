---
title: First Step
weight: 1
---

## Before We Begin

### Preparing Our Tools
Before starting, we need to prepare the necessary tools for fine-tuning Stable Diffusion with LoRA.

## References
Here are some useful resources to guide us through the process:

*   [Fine-Tuning Stable Diffusion with LoRA](https://machinelearningmastery.com/fine-tuning-stable-diffusion-with-lora) (Webpage)
*   [Fine-Tune Stable Diffusion with LoRA for as Low as $1](https://youtu.be/Zev6F0T1L3Y?t=458) (Video)
*   [Pokémon Dataset](https://huggingface.co/datasets/svjack/pokemon-blip-captions-en-zh) (Dataset)
*   [Diffusers GitHub Repository](https://github.com/huggingface/diffusers/) (GitHub)
*   [How to Fine-Tune with LoRA by Hugging Face](https://huggingface.co/docs/diffusers/en/training/lora) (Documentation)

## Required Tools

To set up our working environment, we need the following tools:

* [A GPU server](https://vast.ai) - To run our code. In this guide, we use [vast.ai](https://vast.ai).
* [PuTTY](https://www.putty.org/) - To connect to the server via SSH.
* [WinSCP](https://winscp.net/eng/download.php) - For easy file transfer between the server and local PC.
* A [Hugging Face](https://huggingface.co/) account.
* Python 3 - Ensure Python 3 is installed on your system.

## Connecting to the Server

### Logging into the Server
1. Go to [https://cloud.vast.ai](https://cloud.vast.ai).
2. Register and ensure your account has sufficient credit.

### Creating an SSH Connection
1. Install [PuTTY](https://www.putty.org/) as mentioned above. (Ubuntu and macOS users can use the terminal instead. Windows users can also use PowerShell, but PuTTY is recommended.)
2. Watch the video below to learn how to create an SSH key using **PuTTYgen**:

   [![PuTTY](https://img.youtube.com/vi/KraLVgFS4vU/0.jpg)](https://www.youtube.com/watch?v=KraLVgFS4vU)

3. After generating your SSH key, add the public key to your **Vast.ai** account as shown below:

   ![Public Key Setup](vasi_key.png)

### Selecting a Server

Once logged into Vast.ai, you will see an environment similar to the following:

![Server Selection](vast.png)

1. **Choose a Template:**
   - It is recommended to select **Ubuntu 22.04**.
   - Alternatively, choose another OS if needed.
2. **Choose a GPU:**
   - For training and testing, **NVIDIA RTX Series** GPUs are recommended.
   - Good options include **RTX 3060, RTX 3070, and RTX 3090**, depending on your computational requirements.
3. **Select Server Type:**
   - **On-demand servers** are recommended since **interruptible servers** may be disconnected unexpectedly.
4. After selecting your server, click **RENT** to proceed.
5. You will be redirected to a page that looks like the following.
