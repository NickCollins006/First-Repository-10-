# First-Repository-10-
#11-2-15
#Filename: P05_Strings.py
#Author: Nicholas Collins
#Date: 10/12/15
#Purpose: To solidify my knowledge of string manipulation

#Activity 1
user = input('Insert a famous quote: ')
for i in range(1, 4):
    index = int(input('Input an integer: '))
    slice1 = user[index:]
    slice2 = user[:index]
    slice3 = user[::index]
    if (index < len(user)):
        print('Original string: ' + user)
        print('Slice 1: ' + slice1)
        print('Slice 2: ' + slice2)
        print('Slice 3: ' + slice3)
    else:
        print('Please insert a integer lower than: ', len(user))
        continue

    
print()
#Activity 2
user2 = input('Insert another famouse quote(min 4 words): ')
print('Original string: ', user2)
num = 0
while (num < 3):

    if (num == 0):
        split1 = user2.split()
        print('First-split: ' , split1)
        num += 1
    elif (num == 1):
        split2 = (split1[0]+ split1[2]+ split1[3])
        print('Second-Cadenation: ' ,split2)
        num += 1
    elif (num == 2):
        char = '//'
        join1 = char.join(split1)
        print('Third-Joining of strings: ',join1)
        num += 1
        
