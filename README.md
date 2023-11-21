本文档内包含VIM的插件及相关配置

1. basic_vimrc
  该文件中包含基本配置信息，可以放于/etc/vimrc中作为全局配置

2. local_vimrc
  该文件中是一些个性配置，包含了个人的基本信息及插件的配置，可以作为个人的配置处理，里面需要根据个人的信息进行一些修正

3. configs.tgz
  该文件是github上一个生成vim配置的项目，另外还包括了不少插件

4. plugins
  该目录中包含了一些基本插件，可以直接解压到~/.vim目录下
  在vim命令模式下执行：
    :PluginInstall

5. 安装vim-go
  安装完vim-go插件后，vim-go本身依赖一些包，在vim命令模块下执行：
    :GoInstallBinaries

6. 编译YouCompleteMe
  安装完YouCompleteMe后，还需要单独编译才能运行YouaCompleteMe：
    cd ~/.vim/bundle/YouCompleteMe
    sh install.py --go-completer
    YouCompleteMe支持多语言，其它语言支持请参考YouCompleteMe源代码目录下的README.md文件。
