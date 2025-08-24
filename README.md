# Programming-Assignment-1
#Alphabet Soup Problem
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
