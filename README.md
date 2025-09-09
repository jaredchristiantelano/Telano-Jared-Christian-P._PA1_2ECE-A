# Telano-Jared-Christian-P._PA1_2ECE-A 

1. **Alphabet Soup Problem**: Create a function that takes a string and returns a string with its letters in alphabetical order.
   
Code Description: This code uses the list() function and turns the string from user input into a list before sorting the characters in alphabetical order using sorted(). After arranging it in order, the list is turned into a string again using the function "".join(). 

Code
```
# Alphabet Soup Problem 

def alphabet_soup(word):                          # Creates a function
    x = list(word)                                # Arranges the characters of a string into a list
    y = sorted(x)                                 # Sorting the list in alphabetical order   
    z = "".join(y)                                # Turning the list into a string again 
    return print(f"The arranged word is {z}")     # Prints out the arranged word

alphabet_soup(word = input("Enter a word: "))     # Gets user input for the string  
```


2. **Emotify Problem**: Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad, and mad with their corresponding emoticon.
   
Code Description: This code first creates a dictionary, entailing words with their corresponding emoticons. The code uses a for loop to look for words in the sentence that are also in the dictionary, which will then be replaced with their corresponding emoticon from the dictionary. 

Code 
```
# Emoticon Problem

emoticons = {                                            # Creates a dictionary
    "smile" : ":)", 
    "grin" : ":D", 
    "sad" : ":((", 
    "mad" : ">:("
}

def emotify(sentence):                                   # Defines the function 
    for word, emoticon in emoticons.items():             # The "for" and "in" was used 
        sentence = sentence.replace(word, emoticon)      # Replaces the words in the sentence with its corresponding emoticon from the dictionary
    print(sentence)                                      # Returns new sentence

sentence = emotify(input("Enter the sentence: "))        # Calls function and gets the sentence from user input
```

3. **Unpacking List Problem**: Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.
   
Code Description: This code gets the list from user input. It then gets the first element, collects the remaining elements using a star operator before the last element of the list. 

Code 
```
# Unpacking List Problem

writeyourcodehere = input("Enter your list (do not use spaces or comma):  ")    # Gets the list from user input

first, *middle, last = writeyourcodehere                                        # Gets the first element, then collects the remaining elements before the last element   
                                                                                # The star (*) operator puts the remaining elements of a list
print(f"first: {first}     middle: {middle}      last: {last}")                 # Prints the three variables                      
```

   
