# DeployVPS


## 下载合并内核, 并执行安装
wget https://raw.githubusercontent.com/Child2015/kernel-ml-5.7.6/master/kernel-ml-5.7.6-1.el7.elrepo.x86_64.rpm.aa
wget https://raw.githubusercontent.com/Child2015/kernel-ml-5.7.6/master/kernel-ml-5.7.6-1.el7.elrepo.x86_64.rpm.ab
wget https://raw.githubusercontent.com/Child2015/kernel-ml-5.7.6/master/kernel-ml-5.7.6-1.el7.elrepo.x86_64.rpm.ac
cat kernel-ml-5.7.6-1.el7.elrepo.x86_64.rpm.a* > kernel-ml-5.7.6-1.el7.elrepo.x86_64.rpm && rm -f kernel-ml-5.7.6-1.el7.elrepo.x86_64.rpm.a* && yum localinstall kernel-ml-5.7.6-1.el7.elrepo.x86_64.rpm

# awk -F\' '/menuentry / {print $2}' /boot/grub2/grub.cfg
# grub2-mkconfig -o /boot/grub2/grub.cfg
# grub2-set-default 1
# grub2-editenv list

# yum autoremove kernel-tools-3.10.0

wget https://raw.githubusercontent.com/Child2015/kernel-ml-5.7.6/master/v2ray.sh
