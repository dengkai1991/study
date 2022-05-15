# 常用命令

## 端口占用
1. 查看端口占用
```
netstat -aon|findstr "8081"
```

2. 查看指定 PID 的进程
```
tasklist|findstr "9088"
```

3. 结束进程

**强制（/F参数）杀死 pid 为 9088 的所有进程包括子进程（/T参数）**
```
taskkill /T /F /PID 9088
```