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
