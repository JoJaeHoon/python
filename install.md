### python install  
 1. `wget https://www.python.org/ftp/python/3.6.4/Python-3.6.4.tgz`  
    - Web Get' wget 웹 상의 파일을 다운로드 받을 때 사용  
    - [python](https://www.python.org/downloads/source/ "python")
 2. `tar xvzf Python-3.6.4.tgz`  
    - 압축 하기 tar -cvzf '압축될 이름' '압축할 파일/폴더명', 압축 풀기 tar -xvzf '압축 해제할 파일'  
 3. `cd Python-3.6.4`  
 4. `./configure`  
    - 소스를 받아서 컴파일할 때 ./configure 스크립트를 이용하여 Makefile 만듬  
    - Makefile : 파일 간의 종속관계를 파악하여 shell 명령이 순차적으로 실행되게 만듬
 5. `make`  
    - 반복적 명령의 자동화로 시간 절약, 관리가 용이  
 6. sudo make install  
    - ERROR : zipimport.zipimporterror can't decompress data zlib not available  
    - sudo apt-get install zlib1g-dev  
    - yum install zlib-devel  
***
### 가상환경 Virtualenv  
Python 개발 환경을 분리시키기 위해 가상 환경사용  
 1. Virtualenv pip로 설치  
    - `sudo pip install --upgrade virtualenv`  
 2. 디렉토리 생성  
    - Linux : `mkdir JProject` / Windows : `md JProject`  
 3. 가상환경 생성  
    - `virtualenv [OPTIONS] DEST_DIR`  
    - ex) `virtualenv venv`, `virtualenv --python=python3.6 venv`  
 4. 가상환경 활성화/비활성화  
    - 활성화  
      - Window : `venv/Scripts/activate`  
      - Linux : `source venv/bin/activate`  
    - 비활성화  
      - deactivate  
 
