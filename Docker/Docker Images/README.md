# Images
## Docker File
Docker file is a test file written in a specific format that docker can understand. It's basically an instruction and argument format.

```FROM  Ubuntu```
    Here everything that is on left side i.e. FROM is instruction and on your right side is called argument to those instruction.

    Whenever docker build images it build the layered architecture. Each line of instructiom creates a new layer in the docker image with just the changes from the previous layer.