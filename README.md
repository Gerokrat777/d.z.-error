

def string_to_int(s):

    try:
        print(int(s))
    except ValueError:
        print('ОШИБКА: невозможно преобразовать "s" в целое число')



def read_file(filename):
    try:
        with open(filename, 'r') as file:
            return file.read()
    except FileNotFoundError:
        print('ошибка: файл  не найден')
    except IOError:
        print('ошибка ввода/вывода при работе с файлом')




def divide_numbers(a,b):
    return a/b
try:
        print(int(a / b))
    except ZeroDivisionError:
        print('ОШИБКА: на ноль делить нельзя')
    except TypeError:
        print('ОШИБКА: аргументы не числа')




def access_list_element(lst, index):

    try:
        print(lst[index])
    except IndexError:
        print('ОШИБКА: индекс {index} вне диапозона списка')
    except TypeError:
        print('ОШИБКА: индекс должен быть целым числом')


