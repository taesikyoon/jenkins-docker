- [jenkins docs](https://www.jenkins.io/doc/book/installing/docker/)
- [jenkins image hub](https://hub.docker.com/_/jenkins/tags)
- [jenkins docker git](https://github.com/jenkinsci/docker)
- [jenkins envs](https://www.jenkins.io/doc/book/pipeline/jenkinsfile/)
- [jenkins aws steps docs](https://plugins.jenkins.io/pipeline-aws/)

# 젠킨스 서버 스크립트 실행만으로 바로 띄우기

# 사용법

```
# 실행권한 추가
chmod +x init.sh

# 스크립트 실행
./init.sh

```

패스워드와 입력과 계정 생성하면 젠킨스 서버 완료

### docker.sock의 권한 문제 발생 시

```
docker exec -u root $container_id chown root:docker /var/run/docker.sock
```
