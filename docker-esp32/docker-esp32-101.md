
docker run --rm -v $PWD:/project -w /project espressif/idf:release-v4.4 idf.py build
|Flag|Description|
|----|---|
|--rm |  tell the Docker Daemon to clean up the container and remove the file system after the container exits|  
|-v $PWD:/project |The -v `$(pwd):/project` option tells the Docker Daemon to start up a volume in our container. Volumes are the best way to persist data in Docker. In this example, we are telling Docker that we want the current directory - retrieved from $(pwd) - to be added to our container in the folder /project.|
|-w /project| Working directory inside the container |
espressif/idf:release-v4.4
idf.py build



 
