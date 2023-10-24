---
next_page: app.md
---

## The command you just ran

Congratulations! You have started the container for this tutorial!
Let's first explain the command that you just ran. In case you forgot,
here's the command:

```cli
docker run --name=makeen-labs -d -p 8080:80 maghbari/makeen-labs:1.2
```

You'll notice a few flags being used. Here's some more info on them:

- `-d` - run the container in detached mode (in the background)
- `-p 8080:80` - map port 8080 of the host to port 80 in the container
- `maghbari/makeen-labs:1.2` - the image to us

## The Docker Dashboard

Before going any further, we want to highlight the Docker Dashboard, which gives
you a quick view of the containers running on your machine. It provides you 
access to container logs, lets you get a shell inside the container, and allows you to easily manage container lifecycle (stop, remove, etc.).


## What is a container?

Now that you've successfully run a container, let's ask ourselves what _is_ a container? Simply put, a container is
another process on your machine that has been isolated from all other processes
on the host machine. Features that have been in Linux for a long time. Docker has worked to make these capabilities approachable and easy to use.

## What is a container image?

When running a container, it uses an isolated filesystem. This custom filesystem is provided 
by a **container image**. Since the image contains the container's filesystem, it must include everything 
needed to run the application - all dependencies, configuration, scripts, binaries, etc. The 
image also contains other configuration for the container, such as environment variables,
a default command to run, and other metadata.

We'll dive deeper into images later on, covering topics such as layering, best practices, and more.

