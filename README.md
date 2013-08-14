gitlab-installer
================

### Installer for GitLab/GitLabHQ on RHEL 6 in China ###


文档是参考老外的脚本进行修改，因为国内的ruby的访问速度很慢，导致脚本很难完整运行，所以我修改了安装步骤，采用国内的淘宝提供ruby源来完成安装。

2013年8月1日：Centos6.4 完成gitlab5.0的安装.目前发现gitlab5.2以上的版本，对git的版本有要求，变化还是很多。直接装gitlab5.4，存在很多问题。

2013年8月2日：比较了一下gitlab5.3和gitlab50的区别，完成了gitlab5.3的安装，邮件的功能，应该是没有配置，后续可以参考邮件功能配置。

Gitlab官方安装文档 https://github.com/gitlabhq/gitlab-recipes/blob/master/install/CentOS_6.md

2013年8月5日：update ruby 2.0，update git 1.8. postfix不需要做任何的设置，默认就可以发送邮件，我已经成功把邮件发送到公司和gmail的邮箱。

2013年8月14日：测试脚本
curl https://raw.github.com/shake/gitlab-installer/master/gitlab.sh | bash

目前可能存在网络的原因，导致安装失败。
