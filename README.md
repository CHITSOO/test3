# test3 - dockerfile로 서버배포

## 1. boilder-plate
스프링부트 CSR RestAPI With Security, JWT, JPA 

## 2. docker
- 도커는 이미지를 만들기 위해 Dockerfile이라는 파일에 자체 DSLDomain-specific language 언어를 이용하여 이미지 생성 과정을 적습니다.

## 3. 실행 과정 순서
- 1. aws 계정 생성 IAM 서비스에서 사용자 생성
2. 리눅스 우분투 20.0.4 t3.mediam

3. cat /etc/lsb-release // 우분투 버전 확인
4. uname -a 리눅스 커널 버전확인


5. sudo apt update
6. sudo apt install -y default-jdk // jdk 11버전 설치
7. java -version // 자바 버전확인


8. sudo apt install -y docker.io // docker 설치
9. sudo systemctl status docker // 도커 기동 여부 확인
9. docker version // 버전 확인


10. ubuntu 계정에 docker 실행권한을 주기 위한 설정 <- sudo 쓰기 귀찮아서.
  sudo chmod 666 /var/run/docker.sock


10. docker images // 도커 이미지 확인
11. docker ps // 실행중인 컨테이너 확인
