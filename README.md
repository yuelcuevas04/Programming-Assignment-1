# Programming-Assignment-1
This programming assignment features three problems namely the Alphabet Soup Problem, Emoticon Problem, and the Unpacking List Problem. Each problem requires implementing algorithms that test your understanding of strings, lists, and basic problem-solving in programming.

# 1.) Alphabet Soup Problem
The Alphabet Soup Problem enables the input word or name into alphabet order. Taking the input string to a new string and arrange it into an alphabetical order.

    letters = input("Enter a word/name: ") #This lets the user to input word or name to be alphabetically arranged
    words = letters.lower()                #Lowers all the case to let the code run smoothly even with Upper case inputs
    word=list(words)                       #This code enables the input string into a list of characters
    word.sort()                            #This code enables the string to be in alphabetical order
    for i in word:                         #A for loop to let the letters be arranged and be printed
        print(i, end="")                   # "i" takes each letter from the list of characters, "end=**" means print everything side by side without spaces 
    
# 2.) Emoticon Problem
The Emoticon Problem enables the user to enter sentence with certain words such as:

Smile - :)

Grin - :D

Sad - :((

Mad - >:( 

This emoticons replaces the words into emoticons after the code runs

    sentence = input("Enter a Sentence: ")     # Enables user to input their sentence that has the certain words
    sentence = sentence.lower()                # Switches everything into lower case

    sentence = sentence.replace("smile", ":)") # Evaluates the sentence and replaces the word smile with :)
    sentence = sentence.replace("grin", ":D")  # Evaluates the sentence and replaces the word grin with :D
    sentence = sentence.replace("sad", ":((")  # Evaluates the sentence and replaces the word sad with :((
    sentence = sentence.replace("mad", ">:(")  # Evaluates the sentence and replaces the word mad with >:(

    print(sentence)                # Prints the sentence after replacing the certain words with emoticons

# 3.) Unpacking List Problem
The Unpacking List Problem enables the user to enter different numbers and the code will separate and print the numbers whether which is first, middle, and last.

    user_input = input("Enter numbers separated by space: ") # A user input for randomly arranged numbers, but the input should be separated by spaces otherwise will be considered as digits number
    array = user_input.split() # The syntax removes space and returns each number into an element in list(array)

    unpack = [] # An empty list to be transferred

    for item in array: # This loop goes through each element "item" inside a the list of "array"
        unpack.append(int(item)) # This code transfers the elements of "array" to "unpack" one by one

    first = unpack[0] # Transfers the element (0) the first value to "first"
    middle = unpack[1:-1] # Transfers the elements 1 to -1 the middle values to "middle"
    last = unpack [-1] # Transfers the element (-1) the last value to "last"

    print("First: ", first) # Prints the First input
    print("Middle: ", middle) # Prints the Middle inputs
    print("Last: ", last) # Prints the Last input
