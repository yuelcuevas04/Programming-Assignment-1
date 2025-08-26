# Programming-Assignment-1
This programming assignment features three problems namely the Alphabet Soup Problem, Emoticon Problem, and the Unpacking List Problem. Each problem requires implementing algorithms that test your understanding of strings, lists, and basic problem-solving in programming.

# 1.) Alphabet Soup Problem
The Alphabet Soup Problem enables the input word or name into alphabet order. Taking the input string to a new string and arrange it into an alphabetical order.

letters = input("Enter a word/name: ") #This lets the user to input word or name to be alphabetically arranged
words = letters.lower() #Lowers all the case to let the code run smoothly even with Upper case inputs
word=list(words) #This code enables the input string into a list of characters.
word.sort() #This code enables the string to be in alphabetical order
for i in word: # A for loop to let the letters be arranged and be printed
    print(i, end="") # "i" takes each letter from the list of characters, "end=**" means print everything side by side without spaces 
    
# 2.) Emoticon Problem
sentence = input("Enter a Sentence: ")
sentence = sentence.lower()

sentence = sentence.replace("smile", ":)")
sentence = sentence.replace("grin", ":D")
sentence = sentence.replace("sad", ":((")
sentence = sentence.replace("mad", ">:(")

print(sentence)

# 3.) Unpacking List Problem
user_input = input("Enter numbers separated by space: ")
array = user_input.split()

unpack = []

for item in array:
    unpack.append(int(item))

first = unpack[0]
middle = unpack[1:-1]
last = unpack [-1]

print("First: ", first)
print("Middle: ", middle)
print("Last: ", last)
