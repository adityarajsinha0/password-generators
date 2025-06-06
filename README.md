import random

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!@#$%^&*()'
length = int(input("Enter the length of the password: "))
password = ""
for i in range(length):
    password += random.choice(chars)

# Determine difficulty level
if length < 6:
    difficulty = "Weak"
    print("Password difficulty level:", difficulty)
elif 6 <= length <= 10:
    difficulty = "Moderate"
    print("Password difficulty level:", difficulty)
else:
    difficulty = "Strong"
    print("Password difficulty level:", difficulty)

print("Generated password:", password)
print("Password difficulty level:", difficulty)
