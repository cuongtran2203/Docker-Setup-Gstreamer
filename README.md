# Docker-Setup-Gstreamer
```
Môi trường thử nghiệm trên hệ điều hành win 10 và sử dụng wsl 2

```
```
Để có thể visual kết quả lên màn hình chúng ta cần cài Xlaunch theo đường dẫn sau :
```
```
https://sourceforge.net/projects/vcxsrv/
```
```
Setup biến DISPLAY=IP:0.0 với IP là IP của máy local
```
```
chạy docker :
```
```
docker run -it image_name -e DISPLAY=$DISPLAY 
```

Cách khởi chạy GUI trong docker tham khảo :


https://dev.to/darksmile92/run-gui-app-in-linux-docker-container-on-windows-host-4kde


mkdir -pv ~/.cache/xdgr
```

```
export XDG_RUNTIME_DIR=$PATH:~/.cache/xdgr


XDG_RUNTIME_DIR=/run/user/10010

```
