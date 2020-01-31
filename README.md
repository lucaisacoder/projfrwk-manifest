# projfrwk-manifest
project framework manifest repo


# USAGE
## Download
  ```
  repo init -u https://github.com/lucaisacoder/projfrwk-manifest.git -b dev -m manifest.xml
  repo sync -j32
  repo forall -c git checkout -b dev origin/dev
  ```
## Components
#### compile OSAL static libary
  ```
  cd ./components/osal
  ./project.py build
  ./project.py install
  ```
  output path: ./public/lib/libosal.a   
               ./public/include/osal

#### compile OSAL unit test
  ```
  cd ./components/osal
  ./project.py unit_test
  ./project.py install
  ```
  output path: ./public/bin/osal_ut
 
#### uninstall
  ```
  cd ./components/osal
  ./project.py uninstall
  ```
