# text-based-adventure
# It's a simple text-based adventure with a humorous touch. 
# code
print("Welcome To the Game!\n")
print("-----------------------")
print("You are in Warora majara village")
print("-----------------------")
print("\nAnswer correctly To win")

def first_question():
    entry1 = input("Do you want to vindaloo or korma?: ")
    if entry1.lower() == "vindaloo":
        print("You are a real man --next question..")
        second_question()
    elif entry1.lower()== "korma":
        print("You loss - bye bye")
        quit()
    else:
        print("Answer not recognised, please try again!!")

def second_question():
    entry2 = input("Want to drink ( beer or Lemonade)? : ")
    if entry2.lower() == "beer":
        print("You chose wisely. Only a beer can kill a vindaloo")
        third_question()
    elif entry2.lower()== "Lemonade":
        print("You big girls blouse! bye bye")
        quit()
    else:
        print("Error occured")
def third_question():
    entry3 = input("Did you put the toilet roll in the fridge last night( y or n): ")
    if entry3.lower() == "y":
        print("Phew, no bum burner for you tomorrow! next question")
        fourth_question()
    elif entry3.lower()== "n":
        print("You are a curry light weight bye bye")
        quit()
    else:
        print("An Error occured")

def fourth_question():
    entry4 = input("Have you got to go to work tomorrow ( yes or no )? : ")
    if entry4.lower() == "yes":
        print("oh no,make sure you wear a nappy")
    elif entry4.lower() == "no":
        print("Ok but make sure you stay near a toilet!")
        sixth_question()
    else:
        print("An Error occured")

def sixth_question():
    entry6 = input("Do you prefer a dessert (yes or no)? : ")
    if entry6.lower() == "yes":
        print("Great! Choose between Gulab Jamun and Mango Kulfi.")
        dessert_choice = input("Enter your dessert choice: ")
        if dessert_choice.lower() == "gulab jamun":
            print("Yummy! You've got good taste.")
            seventh_question()
        elif dessert_choice.lower() == "mango kulfi":
            print("Excellent choice! You have a sweet tooth.")
            seventh_question()
        else:
            print("Invalid dessert choice. Game over!")
            quit()
    elif entry6.lower() == "no":
        print("Skipping dessert? Alright, let's move on.")
        seventh_question()
    else:
        print("An error occurred.")

def seventh_question():
    entry7 = input("What's your favorite color (red, blue, or green)? : ")
    if entry7.lower() == "red":
        print("Nice! Red is a vibrant color.")
        eighth_question()
    elif entry7.lower() == "blue":
        print("Cool! Blue is a calming color.")
        eighth_question()
    elif entry7.lower() == "green":
        print("Green is refreshing! Good choice.")
        eighth_question()
    else:
        print("Invalid color choice. Game over!")
        quit()

def eighth_question():
    entry8 = input("Would you like to explore the nearby forest (yes or no)? : ")
    if entry8.lower() == "yes":
        print("Adventure awaits! Enjoy your journey.")
        winner()
    elif entry8.lower() == "no":
        print("Playing it safe? Alright, have a relaxing time.")
        quit()
    else:
        print("An error occurred.")

def fifth_question():
    entry5 = input("Can you pay the bill ( yes or no)? : ")
    if entry5.lower() == "yes":
        print("Congrats you're a star!")
        winner()
    elif entry5.lower() == "no":
        print("Well, get ready to do the washing up!")
        quit()
    else:
        print("An error occured")
def winner():
    w = "Congrats you won the game... "* 20
    print(w.upper())

first_question()
