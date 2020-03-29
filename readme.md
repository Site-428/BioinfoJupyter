# 环境要求
Ubuntu 18.04及以上
# 预处理
```shell
sudo apt-get update
```
# 部署脚本
```shell
sudo apt install python3 python3-dev curl git npm python3-pip
sudo npm set registry https://registry.npm.taobao.org
curl http://share.bmeonline.cn/root/bioinfo-jupyter/raw/master/bootstrap/bootstrap.py | sudo -EH python3 - --admin bio-admin
```
注意：用户名中字母一律小写
# 启用jupyterlab
```shell
sudo jupyter lab build
```
# R语言添加
在管理员账户中启用终端：
```shell
sudo -E conda install -c https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main r
sudo R
```
```R
> install.packages('IRkernel')
> IRkernel::installspec(user = FALSE)
```
添加R包需要：
```shell
cd /opt/tljh/user/lib/R
sudo chmod o+w library
```