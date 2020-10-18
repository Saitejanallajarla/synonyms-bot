import random
from PyDictionary import PyDictionary 
from datetime import datetime

def introduction():
    greet=["Hey there!This is synonyms bot",
    "Its pleasure seeing you here .I am synonyms  bot..."]
    print(random.choice(greet))

def input_data():
    dict=PyDictionary()
    word=input("enter the word-")
    meaning=dict.meaning(word)
    print(meaning)

def bot():
    introduction()
    name= input("enter ur name")
    print("Hey",name,"whats up","Do u want to know synonyms ")
    input_data()
    print("do you want to know something else","1.yes","2.no")
    choice=int(input("enter the option-"))
    while choice == 1:
     	print("do you want to know something else","1.yes","2.no")
     	input_data()
       

bot()

