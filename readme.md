# ����Ҫ��
Ubuntu 18.04������
# Ԥ����
```shell
sudo apt-get update
```
# ����ű�
```shell
sudo apt install python3 python3-dev curl git npm python3-pip
sudo npm set registry https://registry.npm.taobao.org
curl http://share.bmeonline.cn/root/bioinfo-jupyter/raw/master/bootstrap/bootstrap.py | sudo -EH python3 - --admin bio-admin
```
ע�⣺�û�������ĸһ��Сд
# ����jupyterlab
```shell
sudo jupyter lab build
```
# R�������
�ڹ���Ա�˻��������նˣ�
```shell
sudo -E conda install -c https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main r
sudo R
```
```R
> install.packages('IRkernel')
> IRkernel::installspec(user = FALSE)
```
���R����Ҫ��
```shell
cd /opt/tljh/user/lib/R
sudo chmod o+w library
```