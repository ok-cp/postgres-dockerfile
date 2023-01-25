# 가이드 

1. certs
certs/ca.sh 실행하여 CA 인증서 생성, cert/cert.sh 실행하여 인증서 생성
cn 변경이 필요한 경우 스크립트 수정해야함(localhost 기본)

2. ssl 적용
빌드가 되어도 ssl은 적용되어있지 않으며 ssl-conf 명령어를 실행해야 ssl 이 작동됨.
컨테이너 실행과 동시에 ssl 통신이 필요한 경우, entrypoint에 ssl-conf 를 실행시켜야함.

## 참고
https://dev.to/danvixent/how-to-setup-postgresql-with-ssl-inside-a-docker-container-5f3