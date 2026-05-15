# Simple-calc
import time
def calc():
    print('hi, this is a mini calc, please input the nums =>')
    try:
        a = float(input('num 1:'))
        b = float(input('num 2:'))
        op = input('choose the option (+-/*) :')
        if a == 6 and b == 7 and op == '+':
            for i in range(7):
                print('SIXSEVEN') 
                time.sleep(0.1)
            result = 13
        elif op == '+':
            result = a + b
        elif op == '-':
            result = a - b
        elif op == '*':
            result = a * b
        elif op == '/':
            if b != 0:
                result = a / b
            else:
                print('you cannot / on 0')
                return
        else:
            print("something went wrong. let's try again.")
        print('Your result is:', a, op, b, '=', result)
    except ValueError:
        print('you should input number, not text')
        return
     
calc()
