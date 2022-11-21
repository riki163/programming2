## Лабараторная работа №1 
>Калькулятор 
>[https://replit.com/@riki163/laboratory-work-1#main.py)
```{Python}< >{def ff(a):
    if a.__contains__('.'):
        return float(a)
    else:
        return int(a)


def calculate(a, b, c):
    if c == '+':
        print(a, '+', b, '=', a + b)
    elif c == '-':
        print(a, '-', b, '=', a - b)
    elif c == '*':
        print(a, '*', b, '=', a * b)
    elif c == '/' and (a == 0 or b == 0):
        print('Деление на ноль невозможно')
    elif c == '/':
        print(a, '/', b, '=', a / b)
    else:
        print('Такой операции не существует.')


if __name__ == '__main__':
    num1 = str(input('Введите первое число:'))
    num2 = str(input('Введите второе число:'))
    action = input('Введите действие:')
    num1 = ff(num1)
    num2 = ff(num2)
    calculate(num1, num2, action)

