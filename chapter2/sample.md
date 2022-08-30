1. Use Ubuntu_container
```sh 
>> docker run -p 80:8080 -it ubuntu:20.04 /bin/sh
>> docker run -p 8080:8080 jenkins/jenkins:latest
```
localhost:80と(コンテナ):8080を接続

2. localhost:8080に接続
webブラウザでlocalhost:8080
に接続

3. Jenkinsのパスワードを取得
コンテナのシェルに接続(DockerDesktopなどを用いて)
```
>> cat /var/jenkins_home/secrets/initialAdminPassword
```
でパスワードを取得する

テスト