# docker-demo

---

## bash
A simple example of running a `bash` script in a Docker container. Herein we...

__Demo Instructions:__

- First `cd` to the `bash` directory
- Build the `my-bash-demo-image` Docker image by running `./build.sh`
- Run the container with `docker run --rm my-bash-demo-image`
- Inside `script.sh`, un-comment L#4 and comment our L#3
- Re-run `./build.sh`
- Re-run the container with `docker run --rm my-bash-demo-image`
- Enjoy!

---

## node
Another simple example. This time, we will use Docker to try out our `app` on a
newer version of Node.js

__Demo Instructions__

- First `cd` to the `node` directory
- Build the `my-node-demo-image` Docker image by running `./build.sh`
- Run the container with `docker run --rm -p 8080:8080 my-node-demo-image`
- Point your browser at localhost:8080
- Run `docker ps` to grab the `CONTAINER ID` of running `my-node-demo-image` container
- Run `docker exec -ti <CONTAINER ID> bash`
- Inside the `my-node-demo-image` container run `node -v`
- Run `exit`
- Run `docker stop <CONTAINER ID>`
- Change the version of Node.js in the `Dockerfile`
- Build the `my-node-demo-image` Docker image by running `./build.sh`
- Run the container with `docker run --rm -p 8080:8080 my-node-demo-image`
- Point your browser at localhost:8080
- Run `docker ps` to grab the `CONTAINER ID` of running `my-node-demo-image` container
- Run `docker exec -ti <CONTAINER ID> bash`
- Inside the `my-node-demo-image` container run `node -v`
- Run `exit`
- Run `docker stop <CONTAINER ID>`
- Enjoy!
