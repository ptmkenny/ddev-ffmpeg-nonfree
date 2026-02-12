[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/ptmkenny/ddev-ffmpeg-nonfree/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/ptmkenny/ddev-ffmpeg-nonfree/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/ptmkenny/ddev-ffmpeg-nonfree)](https://github.com/ptmkenny/ddev-ffmpeg-nonfree/commits)
[![release](https://img.shields.io/github/v/release/ptmkenny/ddev-ffmpeg-nonfree)](https://github.com/ptmkenny/ddev-ffmpeg-nonfree/releases/latest)

# DDEV Ffmpeg Nonfree

## Overview

This add-on integrates Ffmpeg Nonfree into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get ptmkenny/ddev-ffmpeg-nonfree
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Ffmpeg Nonfree |
| `ddev logs -s ffmpeg-nonfree` | Check Ffmpeg Nonfree logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.ffmpeg-nonfree --ffmpeg-nonfree-docker-image="ddev/ddev-utilities:latest"
ddev add-on get ptmkenny/ddev-ffmpeg-nonfree
ddev restart
```

Make sure to commit the `.ddev/.env.ffmpeg-nonfree` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `FFMPEG_NONFREE_DOCKER_IMAGE` | `--ffmpeg-nonfree-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@ptmkenny](https://github.com/ptmkenny)**
