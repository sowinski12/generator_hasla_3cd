

6. 1)niepoprawna nazwa zmiennej 
2)niepoprawan nazwa funcji
3)zmienna symbols moze byc zle interpretowana
poprawna wizja kodu
import random

lower = "abcdefghijklmnopqrstuvwxyz"
upper = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
numbers = "0123456789"
symbols = "[]{}()*;/,_-'"

all = lower + upper + numbers + symbols
length = 16
password = "".join(random.choices(all, k=length))

print(password)
