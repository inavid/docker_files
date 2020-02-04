1.- Go to the folder of the service that you need and exec:

  ```
  docker build -t [nombre del container] .
  docker run [nombre del container]
  ```

If you run that way the bin of container should stay active on terminal, if you dont want / need to keep with the log of container you can add -d to the run command to leave it detached

docker run [nombre del container] -d

if you want to map a container port to host port you need to add something like

docker run -p 33060:3306 -d mysql5_7
