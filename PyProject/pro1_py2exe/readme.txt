应用场景：
wxPython：GUI编写
Tkinter：
Pmw：
PyGTK：
pygame：
win32com client：
server：

构建主要步骤：
1. 新建脚本 gui.py
2. 编写编译脚本 setup.py
@e.g
/*****
1)
import distutils
import py2exe
distutils.core.setup(windows=['gui.py'])
2) 如果在安装脚本中用data_files可选项指定了那些额外的文件，
那么py2exe能将这些文件拷贝到dist子目录中。data_files应包含一个元组(target-dir, files)列表，
其中的files是这些额外的文件的列表。诸如配置文件、字体、位图
data_files=[("bitmaps",
["bm/large.gif", "bm/small.gif"]),
("fonts",
glob.glob("fonts\\*.fnt"))],
)
****/
3 编译
python setup.py py2exe