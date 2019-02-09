#  Python Flask - Dockerfiles

1. To build a container in docker, use the following format:

    ```
    docker build -t [CONTAINER NAME] -f [FILE NAME] [LOCATION]
    ```
    ex: `docker build -t micro-system .`
2. To enter a container in docker, use the following format:

    ```
    docker run -it --name=[IMAGE NAME] [CONTAINER]
    ```
    ex: `docker run -it --name micro-sys -p 80:80 micro-system bin/sh`
    
    You also have the option of pulling files from your local machine into the container by adding this flag:
        
3. If you have previously entered a container with a specific image name, you cannot reuse that name. To remove it, use the following format:

    ```
    docker rmi -f [IMAGE NAME]
    ```
    
    If you would like to remove a container, use the following format:
    
    ```
    docker rm [CONTAINER NAME]
    ```
    
4. If you want to save your work, you can commit the container using the following format:

    ```
    docker commit -m "MESSAGE"  [IMAGE NAME] [CONTAINER NAME]
    ```
    
5. To see a list of your docker containers, use the following command:

    ```
    docker images
    ```
    
*******************************************************************************************************************************************
    
6. run the following commands on your local machine to get IP:

    ```
    echo $(ifconfig en0 | grep inet | awk '$1=="inet" {print $2}')
    ```
    
    
    
    
    
    
