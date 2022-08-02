from textblob import TextBlob
def convert(string):
    li= list(string.split())
    return li

str1 = input("Enter a sentence or word : ")
words = convert(str1)
corrected_words = []

for i in words :
    corrected_words.append(TextBlob(i))

print("Wrong Words : ", words)
print("Correct sentence or word is : ")

for i in corrected_words :
    print(i.correct(),end=" ")


Output
--------------------------------------------
Enter a sentence or word :  Wrnog Sentecne
Wrong Words :  ['Wrnog', 'Sentecne']
Correct sentence or word is : 
Wrong Sentence 