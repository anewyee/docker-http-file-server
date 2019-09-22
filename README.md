### Distributives
./distr/database  
./distr/client  
./distr/siebel  

### Usage
```
docker build -t http-file-srvr .
docker run -d -it --name file-srvr -p 8080:80 -v $(pwd)/distr:/usr/share/nginx/html http-file-srvr
```
or run scripts
```
./build.sh
./run.sh
```

### Check
Visit http://localhost:8080  
_for virtual box need to setup port forwarding_

# 打包加载
## 载入

```
cat yee-http-file-server.tar.gz | docker import -  yeechongyeung/m-http-file-server

docker load --input yee-http-file-server.tar.gz 
```
