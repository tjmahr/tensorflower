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
