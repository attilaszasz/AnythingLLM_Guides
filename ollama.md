Ollama is an open-source project that allows you to run large language models (LLMs) locally on your machine. It simplifies the process of downloading, installing, and interacting with various LLMs, providing a user-friendly platform for exploring their capabilities without extensive technical expertise or reliance on cloud-based platforms.

## Installing Ollama

To use Ollama, you need to install it on your machine. You can download the latest version of Ollama from [their GitHub](https://github.com/ollama/ollama?tab=readme-ov-file#windows-preview).  

If you are using Windows, you can use the built in WinGet package manager to install Ollama. Run the following command in Command Prompt or Powershell:

```shell
   winget install -e --id Ollama.Ollama
```

## Downloading a Model

Now that you have Ollama installed, you need to download a model to use with it. You can find a list of available models on the [Ollama Models page](https://ollama.com/library).

If you don't have a dedicated Nvidia or AMD video card, it's recommended that you download a smaller model to avoid performance issues. Gemma2 is a good choice for this purpose. Run the following command in Command Prompt or Powershell to download the Gemma2 model:

```shell
   ollama run gemma2:2b
```

If you do have a dedicated Nvidia or AMD video card, you can download a larger model like llama3.1. Run the following command to download it:

```shell
   ollama run llama3.1:8b
```

You can learn more about using Ollama in this [excellent Youtube series](https://www.youtube.com/watch?v=e3j1a2PKw1k&list=PLvsHpqLkpw0fIT-WbjY-xBRxTftjwiTLB&index=3) by Matt Williams.

---

## Configure AnythingLLM to use Ollama

Choose **Ollama** in the LLM Preference screen.

![Screenshot Ollama Install](/media/AnythingLLM%20Start%20Install%20Ollama.jpg)

If you installed Ollama on the same computer, it will be detected automatically and you can choose the model you downloaded in the previous step.  
If you are connecting to a remote Ollama instance, you will need to enter the IP address and port of the remote machine.

Set `Max Tokens` to 8192. Most newer models support this token limit.

Click on the right arrow to proceed to the next step. 

[Back to main guide](/readme.md)