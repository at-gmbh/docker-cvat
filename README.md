# docker-CVAT images
A docker image of [CVAT](https://github.com/openvinotoolkit/cvat) for [server](https://hub.docker.com/r/atcommons/cvat) and [UI](https://hub.docker.com/r/atcommons/cvat-ui)

#### cvat server
[![CVAT Automated build](https://img.shields.io/docker/cloud/automated/atcommons/cvat)](https://hub.docker.com/r/atcommons/cvat)
[![CVAT Build Status](https://img.shields.io/docker/cloud/build/atcommons/cvat)](https://hub.docker.com/r/atcommons/cvat)
#### cvat ui
[![CVAT UI Automated build](https://img.shields.io/docker/cloud/automated/atcommons/cvat-ui)](https://hub.docker.com/r/atcommons/cvat-ui)
[![CVAT UI Build Status](https://img.shields.io/docker/cloud/build/atcommons/cvat-ui)](https://hub.docker.com/r/atcommons/cvat-ui)


## Supported Tags

* [latest](https://github.com/openvinotoolkit/cvat/blob/master/Dockerfile)
* [1.2.0](https://github.com/openvinotoolkit/cvat/blob/v1.2.0/Dockerfile)


These tags denote version numbers that correspond to the published versions of the CVAT module.

## How to use this image


## Maintaining this Build

When a new version is released, please make a git commit with the modified version in the VERSION file and the corresponding tag with format "vx.x.x".

## Configuration of automated build with docker hub

- add a hooks/build file containing the bash script with docker-compose build
- retag the image (in the bash script) to ${IMAGE_NAME} for docker hub to find the built image afterward
- in automated build configuration, specify a dummy file as dockerfile. It wont be used but must exist.


## Contact

Sebastian Straub (sebastian.straub [at] alexanderthamm.com)
Louis de Gaste  (louis.degaste [at] alexanderthamm.com)

Developed with ❤ at [Alexander Thamm GmbH](https://www.alexanderthamm.com/)

## License


