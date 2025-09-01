# Xinference ARM64 Builder

A GitHub workflow for building ARM64 Docker images of [Xinference](https://github.com/xorbitsai/inference).

## Usage

1. Go to Actions tab in your GitHub repository
2. Select "Build Xinference ARM64 Docker Image"
3. Click "Run workflow"
4. Enter the Xinference tag you want to build (e.g., `v0.11.0`)
5. Click "Run workflow"

The built image will be pushed to:
```
crpi-lxfoqbwevmx9mc1q.cn-chengdu.personal.cr.aliyuncs.com/yuyi_tech/xinference:{tag}-arm64-cpu
```

## Setup

Add these secrets to your GitHub repository settings:
- `ALIYUN_REGISTRY_USERNAME` - Your Aliyun Container Registry username
- `ALIYUN_REGISTRY_PASSWORD` - Your Aliyun Container Registry password

## Features

- Manual trigger with tag selection
- ARM64 platform support
- Uses original Xinference Dockerfile.cpu
- Automatic push to Aliyun Container Registry
- Docker layer caching for faster builds