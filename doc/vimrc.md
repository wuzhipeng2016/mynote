"文件位置C:\Vim
"打开行号
set nu!
"自动折行
set wrap
"开启语法高亮设置
if !exists("syntax_on")
    syntax on
endif
"设置默认语言为C
set filetype=javascript
"设置键映射快捷键
"map <C-F9> :!d:\usr\perl\bin\perl %
"map <C-F11> :!e:\firefox\firefox localhost:8080/perl/%
"设置默认目录
"lcd d:\usr\apache2\htdocs\perl
"TAB距离
filetype plugin indent on
"set nowrap
set tabstop=4
set softtabstop=4
set shiftwidth=4
set expandtab
set autoindent
set smartindent
set nobackup
"颜色类型
"colorscheme greens 


" 设置编码
set encoding=utf-8
set fileencodings=utf-8,chinese,latin-1
if has("win32")
set fileencoding=chinese
else
set fileencoding=utf-8
endif

"解决consle输出乱码
language messages zh_CN.utf-8

" 设置文件编码检测类型及支持格式
set fencs=utf-8,gbk,ucs-bom,gb18030,gb2312,cp936
" 指定菜单语言
set langmenu=zh_CN.utf-8
source $VIMRUNTIME/delmenu.vim
source $VIMRUNTIME/menu.vim
set guifont=DejaVu\ Sans\ Mono:h12 
set guifontwide=新宋体:h12 



"帮助语言
set helplang=cn
set iskeyword+=


