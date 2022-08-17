Describe: wordCounter()

Test: "It should return 1 if a passage has just one word."
Code:
const text = "hello";
wordCounter(text);
Expected Output: 1

Test: "It should return 2 if a passage has two words
Code:
const text = "hello there";
wordCounter(text);
Expected Output: 2

Text: "It should return 0 for an empty string."
Code: wordCounter("");
Expected Output: 0

Test: "It should return 0 for a string that is only spaces."
Code: wordCounter("           ");
Epected Output: 0

Test: "It should not count numbers as words."
Code: wordCounter("hi there 77 19");
Expected Output: 2


Describe: numberOfOccurancesInText()

Test: "It should return 0 occurances of a word for an empty srting."
Code:
const text = "red";
const word = "red";
NumberOfOccurancesInText(word, text);
Epeceted Output: 0

Test: "It should return 1 occurance of a word when the word and the text are the same."
Code:
const text = "red";
const word = "red";
numberOfOccurancesInText(word, text);
Expected Output: 1

Test: "It should return 0 occurances of a word when the word and the text are different."
Code:
const text = "red";
const word = "blue";
numberOfOccurancesInText (word, text);
Expected Output: 0

Test: "It should return the numbr of occurances of a word."
Code:
const text = "red blue red red red green";
const word = "red";
numberOfOccurancesInText(word, text);
Expected Output: 4

Test: "It should return a word match regardless of case."
Code:
const text = "red RED Red green Green GREEN";
const word = "Red";
NumberOfOccurancesInText(word, text);
Expected Output: 3

Test: "It should return a word match regardless of punctuation."
Code:
const text = "Red! Red. I like red, green and yellow.";
const word = "Red";
numberOfOccurancesInText(word, text);
Expected Output: 3

Test: "If an empty string is passed in as a word it should return 0."
Code:
const word = "";
const text = "red RED Red!";
numberOfOccurencesInText(word, text);
Expected Output: 0

Description: wordFrequency()

Test: "It should return 0 if it is an empty string"
Code:
const word = "";
const text = "hi";
wordFrequency(word, text);
Expected Output: 0;


Test: "It should return how many times each word is used in the passage of a text"
Code:
const word = "hi";
const text = "hi there"
wordFrequency(word, text);
Expected Output: 1;

Description: orderByFrequency()

Test:"It should organize the output from most used to least used"
code:
const word1 = "hi";
const word2 = "there"; 
const text = "hi there there";
wordFrequency(word1, word2, text);
Expected Output: hi: 1
                 there: 2