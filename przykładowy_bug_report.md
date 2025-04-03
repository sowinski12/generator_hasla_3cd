poprawny kod:

import random

lower = "abcdefghijklmnopqrstuvwxyz"
upper = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
numbers = "0123456789"
symbols = "[]{}()*;/,_-'"

all = lower + upper + numbers + symbols
length = 16
password = "".join(random.choices(all, k=length))

print(password)


# Raport o blędzie
poprawienie kodu

## Numer / identyfikator błędu
#001


## Tytuł błędu

Błędy składniowe i literówki w kodzie generatora haseł


## Priorytet
Wysoki 


## Platforma / środowisko
window/macos/linus


## Opis
Kod odpowiedzialny za generowanie losowego hasła zawiera błędy składniowe i literówki, które powodują jego niepoprawne działanie. Wymaga poprawy, aby działał zgodnie z oczekiwaniami.

## Kroki do reprodukcji
1)1.	Uruchom skrypt generatora haseł.
	2.	Wystąpi błąd związany z literówką w nazwie zmiennej (number zamiast numbers).
	3.	Nieprawidłowe wywołanie funkcji random.samplef() zamiast random.sample().
	4.	Brak unikalności znaków w haśle z powodu użycia sample() zamiast choices()


## Oczekiwany i rzeczywisty wynik
oczekiwanie:generowanie hasla 
Kod zwraca błąd składniowy lub działa niepoprawnie.

## Zrzut ekranu
![IMG_0369](https://github.com/user-attachments/assets/ad57dd2a-b709-47cf-a872-4f839e06693d)

