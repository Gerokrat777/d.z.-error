

def string_to_int():
    s='привет'
    try:
        print(int(s))
    except ValueError:
        print('ОШИБКА: невозможно преобразовать "s" в целое число')
string_to_int()


file_name = 'out.txt'
def read_file():
    try:
        with open('out.txt', mode='r', encoding='utf-8') as file:
            return file.read()
    except FileNotFoundError:
        print('ошибка: файл  не найден')
    except IOError:
        print('ошибка ввода/вывода при работе с файлом')

read_file()


def divide_numbers():
    a = 10
    b = 0
    try:
        print(int(a / b))
    except ZeroDivisionError:
        print('ОШИБКА: на ноль делить нельзя')
    except TypeError:
        print('ОШИБКА: аргументы не числа')

divide_numbers()


def access_list_element():
    lst = 5
    index = 2,5
    try:
        print(lst[index])
    except IndexError:
        print('ОШИБКА: индекс {index} вне диапозона списка')
    except TypeError:
        print('ОШИБКА: индекс должен быть целым числом')

access_list_element()
