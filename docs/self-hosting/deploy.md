# How to deploy Azolyzer
The official way of deploying Azolyzer is by using [docker](https://www.docker.com/){target=_blank} and [docker-compose](https://docs.docker.com/compose/){target=_blank}. 
## Docker-Compose
In order to deploy Azolyzer by using the recommended way, you need to have [docker](https://www.docker.com/){target=_blank} and [docker-compose](https://docs.docker.com/compose/){target=_blank} installed on the machine, on which azolyzer will run.  
1) First of all you need to get the [docker-compose.yml](https://github.com/Azorimor/azolyzer/blob/develop/docker-compose.yml) file from the [Azolyzer Github repository](https://github.com/Azorimor/azolyzer){target=_blank}. Just download this file or copy the content of the file to a file named **docker-compose.yml** on the machine.  
2) Now you need to edit some of the enviroment variabled in that file to fit your needs. You can see more information on this topic [here](environment.md).  
3) After that open a terminal in the same folder, where this file is located and run the command:
```
docker-compose up -d
```

## Kubernetes
The publicly hosted instance of Azolyzer is deployed using kubernetes. This topic will not be mentioned in the documentation, because you should not deploy a instance for too many servers, but if you know what you are doing, you can use kubernetes related code, which is also available on the [Azolyzer Github repository](https://github.com/Azorimor/azolyzer).