# PythonReNamer
Консольная программа заменяющая имена в каталоге

# Замена имени всех файлов в дериктории

import os

directory = 'C:/ntcn/mo/'
files = os.listdir(directory)
print(files)

for i in files:
    # Формируем путь к ВоркБук(файлу)
    # wb = openpyxl.load_workbook(filename = directory + i)

    # Выбираем рабочий лист
    # sheet = wb['свод']

    # Выводит порядковый номер файла (может пригодитьться)
    # counter = files.index(i)+1

    # Берем файл из списка
    oldName = directory + i

	# Берем значение ячейки 'B3' из текущего файла
    val = sheet['B3'].value

    # Формируем имя
    newName = val + ".xlsx"

    # Переимено
    os.rename(oldName, newName)


