jupyter-notebook-action
=======================
### Install package
- Conda
  ```
  import sys
  !conda install --yes --prefix {sys.prefix} numpy
  ```
- pip
  ```
  import sys
  !{sys.executable} -m pip install numpy
  ```

### DevTunnel
- See [dirkarnez/devtunnel-playground](https://github.com/dirkarnez/devtunnel-playground)

### Web UI
- `https://${Tunnel ID}.devtunnels.ms:8080/`

### Notes
- `sudo chmod -R +x . && ./build.sh` in CI/CD .yaml file is good enough for running docker build on GitHub Action
- too busy - use Docker image instead
  - [jupyter/docker-stacks: Ready-to-run Docker images containing Jupyter applications](https://github.com/jupyter/docker-stacks)
    - [Organization jupyter · Quay](https://quay.io/organization/jupyter)
  - [~jupyter/base-notebook - Docker Image | Docker Hub~](https://hub.docker.com/r/jupyter/base-notebook/)

### Reference
- https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/
