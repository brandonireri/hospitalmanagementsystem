# Run the application
Make sure you have docker installed

## Build docker image 
Build docker docker image with name tag `hospital` using Dockerfile in current working dir
```bash 
sudo docker build -t hospital .
```

## Run docker image created
Run docker image with name tag hospital mapping docker container port 8000 to local machine port 80 `-p 80:8000` in interactive mode using `-it` command
```bash
sudo docker run -it -p 80:8000 hospital:latest
```

## Stop docker container and delete hospital docker image
```bash
sudo docker stop
sudo docker rmi hospital --force
```