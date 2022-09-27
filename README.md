# Guess-The-Word
# Guess-The-Word in Python
# Made By Dhyey Thakkar

import getpass

print('''Hello! Welcome to the 'GUESS THE WORD GAME'.
You will only have 7 attempts to guess the word by letters
and after that, you will have 1 chance to guess the word.
If you fail to do so, Player 1 wins
but if you guess the word Player 2 wins

''')

a = player1 = getpass.getpass(str(prompt = "Player 1 enter a word: "))  # hides user input

print("The word enter by player 1 has", (len(a)), "letters")
spaces = ("_" * (len(a)))
print(f'''{spaces}
''')

print("Player 2 now it's your turn to guess")

letter1 = input("Enter the first letter you think is in the word: ")

if letter1 in a:
    print("Yes, that letter is a correct guess")
    counter1 = a.count(letter1)
    print (f"Count of '{letter1}' in the word is : "+  str(counter1))
    print(f"You have guessed {counter1} out {len(a)} letters")
    spaces = spaces.replace("_", letter1,counter1)
    print(f"These are the letters in the word and they are NOT IN ORDER {spaces}")

    chance = input('''
If you think you know the word then you can enter it.
If you don't want to then type move
''')

    if chance == a:
        print('''Hurray! You have guessed the word
Player 2 Wins''')
        if chance == a:
            exit()
    elif chance == "move":
        pass
    elif chance !=a:
        print('''Wrong guess
''')


else:
    print('''Uh oh! That was a wrong guess.
You have 6 more attempts left
''')
    counter1 = 0


letter2 = input("Enter the second letter you think is in the word: ")

if letter2 in a:
    print("Yes, that letter is a correct guess")
    counter2 = a.count(letter2)
    print (f"Count of '{letter2}' in the word is : "+  str(counter2))
    print(f"You have guessed {counter1 + counter2} out {len(a)} letters")
    spaces = spaces.replace("_",letter2,counter2)
    print(f"These are the letters in the word and they are NOT IN ORDER {spaces}")
    chance = input('''
If you think you know the word then you can enter it.
If you don't want to then type move
''')

    if chance == a:
        print('''Hurray! You have guessed the word
Player 2 Wins''')
        if chance == a:
            exit()
    elif chance == "move":
        pass
    elif chance !=a:
        print('''Wrong guess
''')

else:
    print('''Uh oh! That was a wrong guess.
You have 5 more attempts left
''')
    counter2 = 0

letter3 = input("Enter the third letter you think is in the word: ")

if letter3 in a:
    print("Yes, that letter is a correct guess")
    counter3 = a.count(letter3)
    print (f"Count of '{letter3}' in the word is : "+  str(counter3))
    print(f"You have guessed {counter1 + counter2 + counter3} out {len(a)} letters")
    spaces = spaces.replace("_", letter3,counter3)
    print(f"These are the letters in the word and they are NOT IN ORDER {spaces}")
    chance = input('''
If you think you know the word then you can enter it.
If you don't want to then type move
''')

    if chance == a:
        print('''Hurray! You have guessed the word
Player 2 Wins''')
        if chance == a:
            exit()
    elif chance == "move":
        pass
    elif chance !=a:
        print('''Wrong guess
''')

else:
    print('''Uh oh! That was a wrong guess.
You have 4 more attempts left
''')
    counter3 = 0

letter4 = input("Enter the fourth letter you think is in the word: ")

if letter4 in a:
    print("Yes, that letter is a correct guess")
    counter4 = a.count(letter4)
    print (f"Count of '{letter4}' in the word is : "+  str(counter4))
    print(f"You have guessed {counter1 + counter2 + counter3 + counter4} out {len(a)} letters")
    spaces = spaces.replace("_", letter4,counter4)
    print(f"These are the letters in the word and they are NOT IN ORDER {spaces}")
    chance = input('''
If you think you know the word then you can enter it.
If you don't want to then type move
''')

    if chance == a:
        print('''Hurray! You have guessed the word
Player 2 Wins''')
        if chance == a:
            exit()
    elif chance == "move":
        pass
    elif chance !=a:
        print('''Wrong guess
''')
else:
    print('''Uh oh! That was a wrong guess.
You have 3 more attempts left
''')
    counter4 = 0

letter5 = input("Enter the fifth letter you think is in the word: ")

if letter5 in a:
    print("Yes, that letter is a correct guess")
    counter5 = a.count(letter5)
    print (f"Count of '{letter5}' in the word is : "+  str(counter5))
    print(f"You have guessed {counter1 + counter2 + counter3 + counter4 + counter5} out {len(a)} letters")
    spaces = spaces.replace("_", letter5,counter5)
    print(f"These are the letters in the word and they are NOT IN ORDER {spaces}")
    chance = input('''
If you think you know the word then you can enter it.
If you don't want to then type move
''')

    if chance == a:
        print('''Hurray! You have guessed the word
Player 2 Wins''')
        if chance == a:
            exit()
    elif chance == "move":
        pass
    elif chance !=a:
        print('''Wrong guess
''')
else:
    print('''Uh oh! That was a wrong guess.
You have 2 more attempts left
''')
    counter5 = 0

letter6 = input("Enter the sixth letter you think is in the word: ")

if letter6 in a:
    print("Yes, that letter is a correct guess")
    counter6 = a.count(letter6)
    print (f"Count of '{letter6}' in the word is : "+  str(counter6))
    print(f"You have guessed {counter1 + counter2 + counter3 + counter4 + counter5 + counter6} out {len(a)} letters")
    spaces = spaces.replace("_", letter6,counter6)
    print(f"These are the letters in the word and they are NOT IN ORDER {spaces}")

    chance = input('''
If you think you know the word then you can enter it.
If you don't want to then type move
''')

    if chance == a:
        print('''Hurray! You have guessed the word
Player 2 Wins''')
        if chance == a:
            exit()
    elif chance == "move":
        pass
    elif chance !=a:
        print('''Wrong guess
''')


else:
    print('''Uh oh! That was a wrong guess.
You have 1 more attempts left
''')
    counter6 = 0

letter7 = input("Enter the seventh letter you think is in the word: ")

if letter7 in a:
    print("Yes, that letter is a correct guess")
    counter7 = a.count(letter7)
    print (f"Count of '{letter7}' in the word is : "+  str(counter7))
    print(f"You have guessed {counter1 + counter2 + counter3 + counter4 + counter5 + counter6 + counter7} out {len(a)} letters")
    spaces = spaces.replace("_", letter7,counter7)
    print(f"These are the letters in the word and they are NOT IN ORDER {spaces}")

    chance = input('''
If you think you know the word then you can enter it.
If you don't want to then type move
''')

    if chance == a:
        print('''Hurray! You have guessed the word
Player 2 Wins''')
        if chance == a:
            exit()
    elif chance == "move":
        pass
    elif chance !=a:
        print('''Wrong guess
''')


else:
    print('''Uh oh! That was a wrong guess.
You have no more attempts left
''')

    lastchance = input('''This is your final chance.
Guess the WORD NOW''')

if lastchance == a:
    print('''Hurray! You have guessed the word
Player 2 Wins''')
else:
    print('''Wrong guesss
''')

    counter7 = 0

    print(f'''The word entered by Player 1 was {a}
''')

    print('''Player 2 wasn't able to guess the word.
Player 1 wins''')
