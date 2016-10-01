Desktop Installation

Fresh Ubuntu 16.04 install on VirtualBox

R

- Updated R sources
- Added public key for R sources
- Installed R
- Installed RDtudio
- Installed tidyverse
- Installed 3 more dependencies so tidyverse could install its dependencies.

python

- `sudo apt-get install python-pip python-dev`
- `sudo apt-get install python3-pip python3-dev`

tensorflow

```
export TF_BINARY_URL=https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.10.0-cp35-cp35m-linux_x86_64.whl
sudo -H pip3 install --upgrade $TF_BINARY_URL
```

More R stuff

- `sudo apt-get install libssh2-1-dev`
- installed rmarkdown, knitr, devtools

rstudio/tensorflow

- `Sys.setenv(TENSORFLOW_PYTHON_VERSION = 3)`
- `devtools::install_github("rstudio/tensorflow")`

RStudio project
 - Made this repo on GitHub
 - Installed git so I could clone the repo
 
 
 
***
 
Laptop Installation
 
- installed docker for windows 10
- docker run -d -p 8787:8787 rocker/rstudio
- ran bash as root. installed tidyverse

```
sudo apt-get update -qq
sudo apt-get install libssh2-1-dev
sudo apt-get install python3-pip python3-dev
export TF_BINARY_URL=https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.10.0-cp35-cp35m-linux_x86_64.whl
sudo -H pip3 install --upgrade $TF_BINARY_URL
```

- installed devtools
- Sys.setenv(TENSORFLOW_PYTHON_VERSION = 3)
- devtools::install_github("rstudio/tensorflow")
- created my own user 
- commit an image

Created a partition on my host (Windows) machine. Opened docker settings and made the partition a shared volume. Use this volume as a mounted space for the docker container so work gets saved.

```
docker run -d -p 8787:8787 -v //t/:/home/tj/scratch tjmahr/rtensorflow bash //etc/services.d/rstudio/run
```

Opened http://localhost:8787/

Had to install knitr and rmarkdown.

I forgot to configure git.
