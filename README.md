# python-doc

## 安装pyenv
curl -L https://gitee.com/xinghuipeng/pyenv-installer/raw/master/bin/pyenv-installer | bash

## 设置环境变量
cat >>/root/.bashrc<<'EOF'
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"
export PATH="$PYENV_ROOT/shims:$PATH"
eval "$(pyenv init -)"
EOF
 
source /root/.bashrc

## 安装指定版本python
yum install readline-devel,sqlite-devel
pyenv install 3.12.3

## 创建虚拟环境
pyenv virtualenv 3.1.23 devlope
