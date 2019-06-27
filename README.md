## 0. Install Vim
```ruby

sudo yum install cscope ncurses ncurses-devel ncurses-libs ncurses-base python-libs ruby-devel python34 python34-pip python-devel python3-devel python34-devel

git clone git@github.com:vim/vim.git

cd vim

make distclean

./configure \
--enable-multibyte \
--enable-perlinterp \
--enable-rubyinterp \
--enable-pythoninterp \
--enable-python3interp \
--with-python-config-dir=/usr/lib64/python2.7/config \
--with-python3-config-dir=/usr/lib64/python3.4/config-3.4m \
--enable-cscope \
--enable-gui=auto \
--with-features=huge \
--with-x \
--enable-fontset \
--enable-largefile \
--disable-netbeans

make -j 20
sudo make install
```
----
## 1. Set up Vundle:
```ruby
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
----
## 2. Install Plugins:

Launch vim and run 
```ruby
:PluginInstall
```
To install from command line: 
```ruby
vim +PluginInstall +qall
```
----
## 3. Install the YouCompleteMe plugin
```ruby
sudo yum install gcc-c++ cmake python-devel
cd ~/.vim/bundle/YouCompleteMe && python ./install.py
```

----
Reference:
https://github.com/chusiang/vimrc
