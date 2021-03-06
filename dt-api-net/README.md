# Docker - dt-api-net

This folder contains elements that we need to build or configure our dt-api-net within Docker.

### How to build ?

Firstly, we need to get dt-api-net project:

<i> git clone https://github.com/PawelBalcerek/dt-api-net.git </i>

Then we can step into project's folder:

<i> cd dt-api-net </i>

Now if we configured Docker properly, we can use a command below:

<i> docker image build -t dt-api-net:\<image-tag\> . </i>

### How to import configs ?

Get in the config directory:

```shell script
cd config
```

Create a config within Docker:

```shell script
docker config create <config-name> <config-file>
```

Example with appsettings.json:

```shell script
docker config create dt-api-net-properties appsettings.json
```
