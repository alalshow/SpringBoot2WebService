# SpringBoot2 WebService

## 이 코드 그대로 로컬에 돌리면 글등록 forbidden 403 error 발생
* 해결방법: http://localhost:8080/h2-console 에 접속하여 모든 user의 권한을 USER로 변경해야함
    * query문: update user set role ='USER';
    * 로그아웃 후 다시 로그인 

## ec2 서버 상태 확인

### codedeploy 배포 로그 확인
* tail -f /opt/codedeploy-agent/deployment-root/deployment-logs/codedeploy-agent-deployments.log

### 스프링부트 로그확인 배포 로그 확인
* vim ~/app/step3/nohub.out

### 자바 어플리케이션 실행 확인
* ps -ef | grep java

## 최신 코드로 업데이트 참고 문서
* 문서: https://jojoldu.tistory.com/539
* 코드: https://github.com/jojoldu/freelec-springboot2-webservice/tree/version/2020-12-11
* 변경될 도구들의 버전은 다음과 같습니다.
    * Spring Boot 2.4.1
    * Gradle 6.7.1
    * IntelliJ IDEA 2020.3
    * Junit5