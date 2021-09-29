FROM rockylinux/rockylinux:8.4
COPY centos_8.4.2105_extras_x86_64_os.repo /etc/yum.repos.d/
COPY centos_8.4.2105_powertools_x86_64_os.repo /etc/yum.repos.d/
RUN dnf -y install centos-release-openstack-victoria
RUN dnf -y upgrade
RUN dnf -y install python3-openstackclient
RUN dnf -y install bash-completion vim
