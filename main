import random
import time


eng_words = [„Cześć”, „Pa”, „Zadanie”, „Program”]
fr_words = ['Salut','Au revoir','Tâche', 'Programme']
score = 0

mode = input("Wybierz tryb: 0 - dodawaj nowe słowa, 1 - trenuj: \n")
while ((mode != '0') and (mode != '1')):
    mode = input("Nieprawidłowy dymbol! Wybierz 0 lub 1. (0 dodaje nowe słowa, a 1 umożliwia naukę) \n")

if mode == "1":
    print("Przetłumacz jak najwięcej słów! Masz 10 prób!")
    for i in range(10):
        number = random.randint(0, len(eng_words)-1)
        print("Jak powinniśmy tłumaczyć: " + eng_words[number])
        if input() == fr_words[number]:
            print("Świetnie!!!")
            score += 1
        else:
            print("Nie, niezupełnie... Właściwe słowo to - " + eng_words[number])
else:
    word = input("Wpisz angielskie słowo: ")
    translate = input("Wpisz tłumaczenie tego słowa: ")
    if len(word) > 0 and len(translate) > 0:
        eng_words.append(word)
        fr_words.append(translate)
        print("Słowo zostało pomyślnie dodane!")
