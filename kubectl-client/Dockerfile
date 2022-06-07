FROM rockylinux/rockylinux:latest
RUN dnf -y upgrade
RUN dnf -y install bash-completion
RUN dnf -y install vim
RUN curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
RUN mv kubectl /usr/local/bin/
RUN chmod +x /usr/local/bin/kubectl
RUN kubectl completion bash > /etc/bash_completion.d/kubectl
RUN dnf -y install git

