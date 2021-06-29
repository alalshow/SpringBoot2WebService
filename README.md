# SpringBoot2WebService
springboot2 webservice start

## ec2 서버 상태 확인

### codedeploy 배포 로그 확인
tail -f /opt/codedeploy-agent/deployment-root/deployment-logs/codedeploy-agent-deployments.log

### 스프링부트 로그확인 배포 로그 확인
tail -f /opt/codedeploy-agent/deployment-root/deployment-logs/codedeploy-agent-deployments.log

### 자바 어플리케이션 실행 확인
ps -ef | grep java