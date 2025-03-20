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
    --editor-model openrouter/deepseek/deepseek-chat
```

## Customization
You can install dependencies that you rely on by modifying
[Containerfile](share/contaider/env/Containerfile)

