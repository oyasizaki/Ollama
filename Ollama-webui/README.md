## Standard Installation

### If Ollama is on your computer, use this command:

```shell
docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
```


### If Ollama is on a Different Server, use this command:

To connect to Ollama on another server, change the OLLAMA_BASE_URL to the server's URL:
```shell
docker run -d -p 3000:8080 -e OLLAMA_BASE_URL=https://example.com -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
```
After installation, you can access Open WebUI at http://localhost:3000. Enjoy! 😄



## Customized Port connection

```shell
docker run -d -p 3000:8080 -e OLLAMA_BASE_URL=http://127.0.0.1:11435 -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
```
After the completion of the ollama-webui downloading and installing

Access the ollama-webui in the browser
```shell
localhost:3000
```


`Now Follow the instructions in the images`

click on the shown icon in the image
![1](https://github.com/oyasizaki/Ollama/assets/118342512/8e3c55bb-77ca-4d1f-a708-80f98b846b5d)

* Follow the 1st step to navigate to connections settings
* Enter your IP address as shown in the image at step 2
* click on the save button as shown in the step 3
* Refresh by clicking on the refresh icon shown in the step 4
![Screenshot 2024-04-18 065514](https://github.com/oyasizaki/Ollama/assets/118342512/fd1b475d-0f24-4142-8ccd-cb9aa9722ea5)

Now you will be able to see the llm models as shown in the image below
![Screenshot 2024-04-18 065857](https://github.com/oyasizaki/Ollama/assets/118342512/90c5292b-b8dd-4ffa-b158-da5f3a23d2bf)

## UI
![image](https://github.com/oyasizaki/Ollama/assets/118342512/2d133de9-695b-4d01-92ce-b038159a561b)

