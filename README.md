# Programming-Assignment-1
This programming assignment features three problems namely the Alphabet Soup Problem, Emoticon Problem, and the Unpacking List Problem.
The Alphabet Soup Problem enables the input word or name into alphabet order. Taking the ne
**#Alphabet Soup Problem**
letters = input("Enter a word/name: ")
words = letters.lower()
word=list(words)
word.sort()
for i in word:
    print(i, end="")
    
#Emoticon Problem
sentence = input("Enter a Sentence: ")
sentence = sentence.lower()

sentence = sentence.replace("smile", ":)")
sentence = sentence.replace("grin", ":D")
sentence = sentence.replace("sad", ":((")
sentence = sentence.replace("mad", ">:(")

print(sentence)

#Unpacking List Problem
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
