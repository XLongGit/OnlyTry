Ӧ�ó�����
wxPython��GUI��д
Tkinter��
Pmw��
PyGTK��
pygame��
win32com client��
server��

������Ҫ���裺
1. �½��ű� gui.py
2. ��д����ű� setup.py
@e.g
/*****
1)
import distutils
import py2exe
distutils.core.setup(windows=['gui.py'])
2) ����ڰ�װ�ű�����data_files��ѡ��ָ������Щ������ļ���
��ôpy2exe�ܽ���Щ�ļ�������dist��Ŀ¼�С�data_filesӦ����һ��Ԫ��(target-dir, files)�б�
���е�files����Щ������ļ����б����������ļ������塢λͼ
data_files=[("bitmaps",
["bm/large.gif", "bm/small.gif"]),
("fonts",
glob.glob("fonts\\*.fnt"))],
)
****/
3 ����
python setup.py py2exe