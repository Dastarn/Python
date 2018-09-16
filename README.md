# Python
Automatization
Перемещение файлов из одной директории в другую с указанием расширения
import shutil, os, glob

source = 'F:\Новая папка'
dest1 = 'F:\Новая папка (2)'


files = os.listdir(source)

for txt_file in glob.glob(source+"\\*.txt"):
    shutil.copy2(txt_file, dest1)
