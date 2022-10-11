# YaraHunter Docker Extension

## How to install in Docker Desktop ?
*Note: Method to install this extension will change once SecretScanner extension is approved and published by Docker team*

1. Pull the extension image in local
```
docker pull deepfenceio/yarahunter-extension:latest
```

2. Install the extension, make sure Docker Desktop is installed and running
```
docker extension install deepfenceio/yarahunter-extension:latest
```

Enable Docker Extensions
## Insider Preview

<img width="1377" alt="image" src="https://user-images.githubusercontent.com/18168330/194485464-ab8e402f-8e07-4a0c-86e5-3dae39623df8.png">

<img width="1376" alt="image" src="https://user-images.githubusercontent.com/18168330/194485514-4991ccee-15a4-4df4-b407-c57a2a77d372.png">



## DEVELOPMENT

## Enable hot reloading

cd ui

npm start

docker extension dev ui-source deepfenceio/yarahunter-extension http://localhost:3000
                                   

  
## Open Chrome Dev Tools
  
In order to open the Chrome Dev Tools for your extension when clicking on the extension tab, run:

docker extension dev deepfenceio/yarahunter-extension

Each subsequent click on the extension tab will also open Chrome Dev Tools. To stop this behavior, run:

docker extension dev reset deepfenceio/yarahunter-extension



## Change the backend service code

 make build-extension
    
 make update-extension                            
  
ref: https://www.docker.com/blog/build-your-first-docker-extension/
