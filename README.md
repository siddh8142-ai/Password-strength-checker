# Password-strength-checker
it just checks wheter your password has alphabets digits and minimum 8 characters
password=input()

upper=False
lower=False
digits=False

for elem in password:
    if elem <="z" and elem >="a":
        lower=True
    elif elem<="Z" and elem >="A":
        upper=True
    elif elem <= "9" and elem >="0":
        digit=True

if len(password) >=8 and upper and lower and digit:
    print("Strong Password")
else:
    print("Weak Password")
