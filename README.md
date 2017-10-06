# cwru_davinci_cisst_deps

[![Build Status](https://travis-ci.org/cwru-robotics/cwru_davinci_cisst_deps.svg?branch=master)](https://travis-ci.org/cwru-robotics/cwru_davinci_cisst_deps)

This is is the dvrk minim requirements of the JHU-CISST-SAW repository. The original [JHU-CISST-SAW](https://github.com/jhu-cisst/cisst-saw) has several extra packages which are unneccessary for the dvrk and are consequently not included in this version.

## Installation

This repository must be cloned recursively to include all the submodules.
```
git clone --recursive https://github.com/cwru-robotics/cwru_davinci_cisst_deps.git
```

Once downloaded the packages can be build with catkin tool NOT catkin_make.

## catkin build

The guide to using catkin build is available [here](https://catkin-tools.readthedocs.io/en/latest/). For a quick start after initializing the catkin workspace, use the following commands in bash:
```
catkin config --profile release -x _release
# switch to newly created release profile
catkin profile set release
# set default CMake build type
catkin config --cmake-args -DCMAKE_BUILD_TYPE=Release
# build
catkin build
# set environment variables - MAKE SURE YOU SOURCE THE RIGHT FILE (debug vs. release)
source devel_release/setup.bash
```




