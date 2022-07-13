# passwordgenerator
## A password generator tool to create unique and strong passwords for security of all accounts.






import random

print("Welcome to Adrianna's Password Generator")

chars = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz1234567890-_=+!@#$%^&*()~|\<>.?/'

number = input('Amount of passwords to generate: ')
number = int(number)

length = input('Input your password length: ')
length = int(length)

print('\nhere are your passwords:')

for pwd in range(number):
    passwords =''
    for c in range(length):
        passwords += random.choice(chars)
    print(passwords)
