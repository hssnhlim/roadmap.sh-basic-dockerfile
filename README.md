# roadmap.sh-basic-dockerfile

**Requirements**

The Dockerfile should be named Dockerfile.
The Dockerfile should be in the root directory of the project.
The base image should be alpine:latest.
The Dockerfile should contain a single instruction to print “Hello, Captain!” to the console before exiting.

**If you use Window**
Run this code on Window Terminal
```
mkdir hello-captain
cd hello-captain
echo FROM alpine:latest > Dockerfile
echo ENV NAME=Captain >> Dockerfile
echo CMD ["sh", "-c", "echo Hello, $NAME!"] >> Dockerfile
```
This will create `hello-captain` folder and add the code to `Dockerfile` file.

Next, we need to build the Docker image and run it (ensure you have downlaoded Docker):
```
docker build -t hello-captain .
docker run --rm hello-captain
```

This will print `Hello, Captain!` on your terminal.

You can change the name variable by doing this:
```
docker run --rm -e NAME=yourName hello-captain
```

The output will look like this:

`Hello, yourname!`

https://roadmap.sh/projects/basic-dockerfile



