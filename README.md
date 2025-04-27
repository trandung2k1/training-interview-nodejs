1. Cài jenkins bằng docker

```js
docker run -d --name jenkins -p 8080:8080 -p 50000:50000 --volume jenkins-data:/var/jenkins_home jenkins/jenkins:lts
docker exec -it --user root jenkins bash
apt-get install -y docker.io

```

2. Thêm webhook vào repo github

```js
/github-webhook/;
```

3. Tạo item

```js
Chọn NewItem
Chọn Freestyle project
Source Code Management chọn Git, paste link git vào
Triggers chọn GitHub hook trigger for GITScm polling
```
