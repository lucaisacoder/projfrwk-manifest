# projfrwk-manifest
project framework manifest repo

![](https://img.shields.io/badge/license-MIT%2FApache--2.0-blue)


# USAGE
## Download
  ```
  $ repo init -u https://github.com/lucaisacoder/projfrwk-manifest.git -b develop -m manifest.xml
  $ repo sync -j32
  $ repo forall -c git checkout -b develop origin/develop
  ```
## Components
#### compile OSAL static libary
  ```
  $ cd ./components/osal
  $ ./project.py build
  $ ./project.py install
  ```
  output path:<br>
  ./public/lib/libosal.a
  ./public/include/osal
  
#### compile OSAL unit test
  ```
  $ cd ./components/osal
  $ ./project.py unit_test
  $ ./project.py install
  ```
  output path: <br>
  ./public/bin/osal_ut
 
#### uninstall
  ```
  $ cd ./components/osal
  $ ./project.py uninstall
  ```
