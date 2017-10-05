# drone-aws-device-farm-report

Drone plugin to see the status of a test run in AWS Device farm. For the
usage information and a listing of the available options please take a look at
[the docs](DOCS.md).

## Build

Build the binary with the following commands:

```
drone exec
```

## Docker

Build the docker image with the following commands:

```
drone exec
docker build --rm=true -t kowalatech/drone-aws-device-farm-report .
```
## Usage

Execute from the working directory:

```sh
docker run --rm \
  -e AWS_ACCESS_KEY_ID=<accesskeyid> \
  -e AWS_SECRET_ACCESS_KEY=<accesskey> \
  -e PLUGIN_REGION=<region> \
  -e PLUGIN_RUN_NAME=<runname> \
  -e PLUGIN_TEST_PROJECT=<testsproject> \
  -v $(pwd):$(pwd) \
  -w $(pwd) \
  kowalatech/drone-aws-device-farm-report
```
