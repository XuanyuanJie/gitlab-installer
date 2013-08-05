gitlab-installer
================

### Installer for GitLab/GitLabHQ on RHEL 6 in China ###


文档是参考老外的脚本进行修改，因为国内的ruby的访问速度很慢，导致脚本很难完整运行，所以我修改了安装步骤，采用国内的淘宝提供ruby源来完成安装。

2013年8月1日：Centos6.4 完成gitlab5.0的安装.目前发现gitlab5.2以上的版本，对git的版本有要求，变化还是很多。直接装gitlab5.4，存在很多问题。

2013年8月2日：比较了一下gitlab5.3和gitlab50的区别，完成了gitlab5.3的安装，邮件的功能，应该是没有配置，后续可以参考邮件功能配置。

Gitlab官方安装文档 https://github.com/gitlabhq/gitlab-recipes/blob/master/install/CentOS_6.md

2013年8月5日：update ruby 2.0，update git 1.8.


# su git -c "bundle exec rake gitlab:env:info RAILS_ENV=production"

System information
System:         CentOS release 6.4 (Final)
Current User:   git
Using RVM:      yes
RVM Version:    1.21.17
Ruby Version:   2.0.0p247
Gem Version:    2.0.6
Bundler Version:1.3.5
Rake Version:   10.0.4

GitLab information
Version:        5.4.0
Revision:       e8d77e2
Directory:      /home/git/gitlab
DB Adapter:     mysql2
URL:            http://node06.chenshake.com
HTTP Clone URL: http://node06.chenshake.com/some-project.git
SSH Clone URL:  git@node06.chenshake.com:some-project.git
Using LDAP:     no
Using Omniauth: no

GitLab Shell
Version:        1.7.0
Repositories:   /home/git/repositories/
Hooks:          /home/git/gitlab-shell/hooks/
Git:            /usr/bin/git
