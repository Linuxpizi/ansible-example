## 使用

1. 首先编辑 `hosts` 文件中的服务器列表

2. 执行部署

```
ansible-playbook -i hosts site.yml
```
3. 一些坑

```
1. 特殊字符需要使用""包裹起来
  例如: 127.0.0.1 ansible_ssh_user=chia ansible_ssh_pass="admin1234$#@!Q" ansible_sudo_pass="admin1234$#@!Q"
2. ansible host 提示 127.0.0.1 不能 ssh 或者 ssh 拒绝链接 这么处理 127.0.0.1 ansible_connection=local
3. 
```
