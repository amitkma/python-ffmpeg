# Python FFmpeg Docker Image

[![Build Status](https://github.com/amitkma/python-ffmpeg/actions/workflows/ci.yml/badge.svg)](https://github.com/amitkma/python-ffmpeg/actions/workflows/ci.yml)

This repository contains a Docker image for Python with FFmpeg installed. This image is designed to provide a lightweight and efficient environment for running Python applications that require FFmpeg.

## Table of Contents

- [Python FFmpeg Docker Image](#python-ffmpeg-docker-image)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Usage](#usage)
    - [Pulling the Image](#pulling-the-image)
    - [Running a Container](#running-a-container)
  - [Development](#development)
    - [Building the Image](#building-the-image)
    - [Pre-commit Hooks](#pre-commit-hooks)
  - [Contributing](#contributing)
  - [License](#license)

## Features

- Python 3.12 and 3.13
- FFmpeg installed
- Lightweight `slim` base image
- Pre-configured for development with pre-commit hooks

## Usage

### Pulling the Image

You can pull the pre-built Docker image from Docker Hub:

```sh
docker pull amitkma/python-ffmpeg:3.12-slim
```

### Running a Container

You can run a container from the pre-built image:

```sh
docker run -it amitkma/python-ffmpeg:3.12-slim
```

This will start a container with Python 3.12 and FFmpeg installed.

## Development

### Building the Image

To build the Docker image locally, run the following command:

```sh
docker build -t python-ffmpeg:3.12-slim 3.12/
```

### Pre-commit Hooks

The repository includes pre-commit hooks for various checks and lints. To install the hooks, run the following command:

```sh
pip install -r requirements.txt
pre-commit install
```

The pre-commit configuration is defined in [.pre-commit-config.yaml](.pre-commit-config.yaml).

## Contributing

We welcome contributions! Please see the [PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md) for guidelines on how to contribute.

## License

This project is licensed under the Apache 2.0 License. See the
[LICENSE](/LICENSE) file for details.

```sh
    Copyright 2025 Sunserg Technologies Pvt Ltd

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```

## Author

[Amit Kumar](https://github.com/amitkma)
