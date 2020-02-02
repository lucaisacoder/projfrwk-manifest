# projfrwk-manifest
project framework manifest repo

![](https://img.shields.io/badge/license-MIT%2FApache--2.0-blue)


# USAGE
## Download
  ```
  $ repo init -u https://github.com/lucaisacoder/projfrwk-manifest.git -b develop -m manifest.xml
  $ repo sync -j32 --fetch-submodules  
  $ repo forall -c git checkout -b develop origin/develop
  ```
## Components
#### compile OSAL static libary
  ```
  $ cd ./components/osal
  $ ./project.py build
  $ ./project.py install
  $ ./project.py uninstall  
  $ ./project.py clean 
  $ ./project.py distclean   
  ```
  output path:<br>
  ./components/osal/installed/include
  ./components/osal/lib/libosal.a
  ./components/osal/lib/CMake
  
#### compile OSAL unit test
  ```
  $ cd ./components/osal
  $ ./project.py build
  $ ./project.py install
  $ ./project.py uninstall  
  $ ./project.py clean 
  $ ./project.py distclean   
  ```
  output path:<br>
  ./components/osal/bin/osal_ut
 
## Cores
#### compile CORE binary
  $ cd ./core/core
  $ ./project.py build
  $ ./project.py install
  $ ./project.py uninstall  
  $ ./project.py clean 
  $ ./project.py distclean   
  ```
  output path:<br>
  ./core/core/bin/core

#### compile CORE unit test
  $ cd ./core/core
  $ ./project.py build
  $ ./project.py install
  $ ./project.py uninstall  
  $ ./project.py clean 
  $ ./project.py distclean   
  ```
  output path:<br>
  ./core/core/bin/core_ut
