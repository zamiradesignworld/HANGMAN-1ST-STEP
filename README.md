# HANGMAN-1ST-STEP

# TODO-1

import random
word_list = ["aardvark", "baboon", "camel"]
chosen_word = random.choice(word_list)

random_index = random.randrange(len(word_list))

print(word_list[random_index])

# Output: aardvark 

# TODO-2
from random import choice, randint
guess = input("Guess the letter:").lower()

L = ['spring', 'summer', 'winter']
sl = choice(L)
n = randint(0, len(sl) - 1)
for i in range(len(sl)):
    if i == n:
        print('?', end='')
        continue
    print(sl[i], end='')

while True:
    f = input('\nВведите букву:s')
    if f == sl[n]:
        print('победа')
        break
    else:
        print('Попробуйте еще')
