# docker-CVAT images

[![CVAT Automated build](https://img.shields.io/docker/cloud/automated/atcommons/cvat)](https://hub.docker.com/r/atcommons/cvat)
[![CVAT Build Status](https://img.shields.io/docker/cloud/build/atcommons/cvat)](https://hub.docker.com/r/atcommons/cvat)
[![CVAT UI Automated build](https://img.shields.io/docker/cloud/automated/atcommons/cvat-ui)](https://hub.docker.com/r/atcommons/cvat-ui)
[![CVAT UI Build Status](https://img.shields.io/docker/cloud/build/atcommons/cvat-ui)](https://hub.docker.com/r/atcommons/cvat-ui)
[![CVAT - License](https://img.shields.io/pypi/l/personio-py)](https://github.com/at-gmbh/personio-py/blob/master/LICENSE)

A docker image of [CVAT](https://github.com/openvinotoolkit/cvat) for server (https://hub.docker.com/r/atcommons/cvat) and UI (https://hub.docker.com/r/atcommons/cvat-ui)


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

Developed with ❤ at [Alexander Thamm GmbH](https://www.alexanderthamm.com/)

## License

    Copyright 2020 Alexander Thamm GmbH

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
