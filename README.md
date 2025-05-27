# contaider
Use [aider](https://aider.chat) inside an
[OCI-container](https://en.wikipedia.org/wiki/Open_Container_Initiative).

## Example usage
```console
$ mkdir my-brainstorming-idea
$ cd my-brainstorming-idea
$ git init .
$ export OPENROUTER_API_KEY="sk-or-v1-deadbeef0badcafe"
$ contaider --architect --model openrouter/deepseek/deepseek-r1 \
    --editor-model openrouter/deepseek/deepseek-chat-v3-0324 \
    --weak-model openrouter/google/gemini-2.0-flash-lite-001
```

## Customization
You can install dependencies that you rely on by modifying
[Containerfile](share/contaider/env/Containerfile)

## Local models
You can use e.g [llama-swap](https://github.com/mostlygeek/llama-swap) and pass e.g.
```console
env OPENAI_API_KEY=placeholder OPENAI_API_BASE=http://host.docker.internal:8686/v1 contaider --architect --model openai/llamacpp-QwQ-32B --editor-model openai/llamacpp-Qwen2.5-Coder-32B-Instruct
```
