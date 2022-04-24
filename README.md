# raspi_kernel

## HOST PC 환경 설정
 - SSH  
~~~
$ sudo apt-get isntall openssh-server
$ sudo ufw allow ssh
~~~

 - docker  
   - docker 설치
    https://docs.docker.com/engine/install/ubuntu/
    sudo docker build -t raspi:imx-1 .
    docker run -it --volume="$PWD/..:/workdir/raspi" raspi:imx-1
 - build 환경 구축
   docker/Dockerfile 참고

## 커널 빌드
 - kernel build
 - firmware에 kernel 모듈 설치
