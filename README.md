# python-for-everybody
maximum = -1
minimum = None
while True:
    num = input('Enter the num: ')
    if num == 'done':
        break
    try:
        num1 = int(num)
    except:
        print('Invalid input')
        continue
    if minimum is None:
        minimum = num1
    if num1 > maximum:
        maximum = num1
    elif num1 < minimum:
        minimum = num1

print('Maximum is', maximum)
print('Minimum is', minimum)
