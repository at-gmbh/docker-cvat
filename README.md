# CVAT DOCKER images
A docker image of [CVAT](https://github.com/openvinotoolkit/cvat) for [server](https://hub.docker.com/r/atcommons/cvat) and [UI](https://hub.docker.com/r/atcommons/cvat-ui)

# Docker Images for CVAT

<table border="0">
  <tr>
    <td><b>cvat server</b></td>
    <td>
      <a href="https://hub.docker.com/r/atcommons/cvat"><img src="https://img.shields.io/docker/cloud/automated/atcommons/cvat" alt="CVAT Automated build"></a>
      <a href="https://hub.docker.com/r/atcommons/cvat"><img src="https://img.shields.io/docker/cloud/build/atcommons/cvat" alt="CVAT Build Status"></a>
    </td>
  </tr>
  <tr>
    <td><b>cvat ui</b></td>
    <td>
      <a href="https://hub.docker.com/r/atcommons/cvat-ui"><img src="https://img.shields.io/docker/cloud/automated/atcommons/cvat-ui" alt="CVAT Automated build"></a>
      <a href="https://hub.docker.com/r/atcommons/cvat-ui"><img src="https://img.shields.io/docker/cloud/build/atcommons/cvat-ui" alt="CVAT Build Status"></a>
    </td>
  </tr>
</table>

Docker Images of [CVAT](https://github.com/openvinotoolkit/cvat) for the [server](https://hub.docker.com/r/atcommons/cvat) and [UI](https://hub.docker.com/r/atcommons/cvat-ui) components.

## Supported Tags

* [latest](https://github.com/openvinotoolkit/cvat/blob/master/Dockerfile)
* [1.2.0](https://github.com/openvinotoolkit/cvat/blob/v1.2.0/Dockerfile)

These tags denote version numbers that correspond to the published versions of the CVAT module.

## How to use this image

To run the CVAT UI image, use:
```
docker run -p 80:80 --name <cvat_ui name> -d atcommon/cvat_ui
```

For an extended description of how to use a CVAT docker image, please go to the official [CVAT installation documentation](https://github.com/openvinotoolkit/cvat/blob/master/cvat/apps/documentation/installation.md).

## Maintaining this Build

When a new version is released, please make a git commit with the modified version in the VERSION file and the corresponding tag with format "vx.x.x".

## Configuration of automated build with docker hub

The usage of docker-compose for automated build by Docker hub involved the following adaptations:

- add a hooks/build file in the repo containing a script with the docker-compose build command, which will replace the docker-hub build phase
- retag the image (in the build script) to ${IMAGE_NAME} (env. variable provided by docker hub) so that docker hub can find the built image afterward.
- in automated build configuration, specify a dummy file as dockerfile. It wont be used for the build but if docker hub requires an existing Dockerfile nevertheless.

## Contact

* Louis de Gaste  (louis.degaste [at] alexanderthamm.com)
* Sebastian Straub (sebastian.straub [at] alexanderthamm.com)

Developed with ❤ at [Alexander Thamm GmbH](https://www.alexanderthamm.com/)

## License

Code released under the [MIT License](./LICENSE). 

We are not affiliated with CVAT. The source code of CVAT is also released under the [MIT License](https://github.com/openvinotoolkit/cvat/blob/develop/LICENSE); however, additional restrictions may apply.
