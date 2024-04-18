
![ollama](https://github.com/oyasizaki/Ollama/assets/118342512/e81475b7-dedc-42a5-961b-41a2d9aae00a)

## Standard Installation

### CPU only 
```shell
docker run -d -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama
```
### With GPU 
```shell
docker run -d --gpus=all -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama
```

## Customized Installation

### Port manipulation
```shell
docker run -d --gpus=all -v ollama:/root/.ollama -p 11435:11434 --name ollama ollama/ollama
```
![Screenshot 2024-04-18 060635](https://github.com/oyasizaki/Ollama/assets/118342512/65739b11-cd0b-42d2-940f-059b77bae95d)

![Screenshot 2024-04-18 061004](https://github.com/oyasizaki/Ollama/assets/118342512/56829f8d-c228-459f-aac4-279818247375)

### Downloading the LLM models
```shell
docker exec -it ollama ollama run {model name}
```
for example
```shell
docker exec -it ollama ollama run llama2
```

### Checking the existing LLM models
for example
```shell
docker exec -it ollama ollama list
```
