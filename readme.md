# AnythingLLM Setup Guide

This guide is intended to help _non-technical_ users set up [AnythingLLM](https://anythingllm.com) on their computer.

## What is AnythingLLM?

AnythingLLM is the easiest to use, all-in-one AI application that can do RAG, AI Agents, and much more with no code or infrastructure headaches.

## Why use AnythingLLM?

AnythingLLM is the easiest to use, all-in-one AI application that can do RAG, AI Agents, and much more with no code or infrastructure headaches. You can use it as a zero-setup, private, and all-in-one AI application for local LLMs, RAG, and AI Agents without requiring any painful infrastructure setup. Additionally, it offers flexible customization options and support for various models and services, providing you with the flexibility to use the tools that suit your needs.

## Installing on desktop

Choose the appropriate version for your operating system:

[Download AnythingLLM](https://anythingllm.com/download)

> **Note:** On Windows, there is a warning when downloading that it's a potentially dangerous file and it's prevented from saving. Do it anyway :).

### Installation & configuration

Run the installer.  
Wait for a looooong time :)

When finished, start the app. You will be greeted with a welcome screen. Click on **Get started** to proceed to the next screen:

![AnythingLLM LLM Preference Screenshot](/media/AnythingLLM%20Start%20Install%20Built%20In.jpg)

On the LLM Preference screen, choose your desired provider. Follow the specific instructions for the provider you chose:
- [Groq](groq.md)
- [Google Gemini](gemini.md)
- [AnythingLLM](builtin.md) (Buit in [Ollama](https://ollama.com/))
- [Ollama](ollama.md) (Self-hosted)


Read the Data Handling & Privacy statement and click on the right arrow again.

You can skip the survey, or you can fill it out if you want to help improve the app.

In the next step you will create your first workspace. Give it a name and click on the right arrow.

![AnythingLLM Workspace Screenshot](/media/AnythingLLM%20Create%20Workspace.jpg)

Click on the right arrow to proceed to the next step.
This will take you to the main screen of the app. On the first run there will be a welcome message with some useful information. Read it.

![AnythingLLM Welcome Screenshot](/media/AnythingLLM%20Welcome.jpg)

Click on the workspace you just created. This will take you to the workspace screen and you can start chatting!

![AnythingLLM Workspace Chat Screenshot](/media/AnythingLLM%20Chat.jpg)

> If you chose the built in provider, at this point when attemting to chat, you will see an error response:  
> `Ollama call failed with status code 400: model is required`.  
> 
> Please [download a model](/builtin_models.md).

Enjoy!

## Basic configuration

### Improving the system prompt

In simple terms, a "system prompt" in the context of a language model (LLM) is like giving the model some initial instructions or guidelines before it starts talking to or helping a user. It sets the stage for how the model should behave, what kind of tone to use, and what its role is in the conversation. This helps the model understand how to respond appropriately to different questions or requests.

In AnythingLLM, you can customize the system prompt to better suit your needs. Here's how:

Click on your workspace.  
Click on the Settings icon (the gear icon) in the right side:

![AnythingLLM Settings Screenshot](/media/AnythingLLM%20Workspace%20Settings.jpg)

In the settings screen, click on the **Chat Settings** tab:

![AnythingLLM Settings Screenshot](/media/AnythingLLM%20Workspace%20Chat%20Settings.jpg)

Scroll down to the **Prompt** section. Here you can customize the system prompt.

Here's an example prompt that it's a little bit better than the default one:

```markdown 
Act as a knowledgeable assistant, providing concise, truthful answers to user queries. 
Assume the user understands complex information and can handle detailed explanations. 
When uncertain, state 'I'm not sure' or 'I don't have enough information.' 
Always maintain a neutral tone. 
Whenever possible, provide references to support the information provided. 
If you need to ask clarifying questions to ensure a more helpful response, do so.
```

### Setting the temperature

This setting controls how "creative" your LLM responses will be.  
The higher the number the more creative.  
For some models this can lead to incoherent responses when set too high.

Recommended: **0.5**