FROM dockerpull.com/python:3.12.5

RUN apt update && \
    apt install -y build-essential

# COPY requirements.txt to container
ADD requirements.txt /tmp/

# 用清华的源安装必须的package
RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple -r /tmp/requirements.txt