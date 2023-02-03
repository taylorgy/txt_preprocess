# txt_add_quations

## 功能
- 给txt文件中的每一行加上前后双引号，并在末尾加两个空格，以方便markdown编辑。
- 如果安装了`pyperclip`包，则将修改后的文本直接复制到剪贴板方便粘贴；
  - 可通过`pip install pyperclip`安装。
- 否则将修改后的文本保存为在原目录下【原文件名_new.txt】中。
  - 保存编码默认为utf-8；读取文件编码为ANSI。

## 使用
- 直接拖拽txt文件至.py文件运行
- 在命令行中输入文件路径作为参数
  - `$ python txt_add_quotations.py path/filename.txt`

## 可改进
- 目前只针对txt文件，ass、md文件无法直接使用
  - 可在程序中将其他文件转换为txt
  - 或添加对其他文件类型读写的支持
- 可尝试在程序内自动安装所需库
  - `os.system()`或`os.popen()`
