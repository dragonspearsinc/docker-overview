## Getting started

Let's make sure that everything is configured properly and test with an nginx image.

1. Open a command prompt
2. `docker run -it --rm -d -p 8080:80 --name web nginx`
3. Open a web browser at [http://localhost:8080](http://localhost:8080)
4. Review the running container `docker ps -a`

Now, let's clean-up the container by stopping it

5. Step 5: `docker stop web`
6. Review that the container does not exist anymore `docker ps -a`


## Time to build our own image and run a container

1.  Open a command prompt in ./sample-nodeapp
2.  docker build -t node-web-app .
2.  docker run -p 49160:3000 -d node-web-app            
3.  docker ps - a
4.  Open a web browser at http://localhost:49160
5.  docker logs <container id>
6.  docker exec -it <container id> /bin/bash
5.  docker stop <container id>


