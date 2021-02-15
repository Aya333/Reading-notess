In this chapter we have learned very important basic elements of HTML, starting with the
1-**Headings:** You can think of them as main points of the pages content, it has six levels of headings and as the number of the headings grow the font weight goes down.
 Syntax: (h1....h6 inside the tag<>).
 
 2-**Paragraphs:** You use them to write a full on text that can be wrapped and move around other elements, it has opening and closing tags.
 Syntax:(simply the letter "P" inside the tag).
 
 3-**Bold:** Using this tag allows some of the words or specific parts that you involve inside this tag to appear in the bold style.
  Syntax:(simply the letter "B" inside the tag).
  
  4-**Italic:** Using this tag allows some of the words or specific parts that you involve inside this tag to appear in Italic style in case you wanted to specify a name or a term inside the full text.
  Syntax:(simply the letter "I" inside the tag).
  
  5-**Sup:** This tag is simply used for specifying characters at the top of a specfic part. Such as suffixes of dates power to in mathemetics...etc.
  Syntax:(simply the letter "sup" inside the tag).
  
 6- **Sub:**  This tag is simply used for specifying characters at the bottom of a specfic part. Such as chemical formulas.
  Syntax:(simply the letter "sub" inside the tag).
  
  7-**BR:** Or line break, from it's name you can tell that it's used to go down one line after a specific word.
  Syntax:(simply the letter "br" inside the tag).
  
  8-**HR:** It creates a visible horizontal line in the page .
  Syntax:(simply the letter "hr" inside the tag).
  
  9-**Strong:** Indicates that the the word after is very important also by default the browser will display it in bold.
  Syntax:(simply the word "strong" inside the tag).
  
  10-**Emphasis:** Emphasises a word that would change the meaning of the whole sentence a bit also by default the browser will display it in Italic .
  Syntax:(simply the letters "em" inside the tag).
  
 11-**Block quote:**It is meant for paragraph sized quotes to differentiate it from the p elements .
  Syntax:(simply the word "Blockquote" inside the tag).
  
  12- **Quote:** For short quotes .
  Syntax:(simply the letter "q" inside the tag).
  
  13-**Abbreviations & Acronyms:** A title attribute on the opening tag is     used to specify the full term.
  Syntax:(simply the letters "abbr" inside the tag).
  
   14-**Citation:** is used to describe a reference to a cited creative work,     and must include the title of that work.
  Syntax:(simply the word "cite" inside the tag).
  
   15-**Definitions:** Used when defining a new term for the first time.
  Syntax:(simply the letters "dfn" inside the tag).
  
   16-**Address:** Used to specify contact details .
  Syntax:(simply the word "address" inside the tag).
   17-**Ins:** Used to underline a specific word or sentence.
  Syntax:(simply the letters "ins" inside the tag).
   18-**Delete:** It crosses the word but does not delete it .
  Syntax:(simply the letter "del" inside the tag).
   19-**S:**Indicates that something is no longer correct .
  Syntax:(simply the letter "S" inside the tag).
  
 ## Those were the most important semantic elements to learn about structuring the webpage.
  
  # CSS:
 - CSS is all about designing the web page to make it presentable and user friendly, as it applies rules to the HTML tags to style them and decide how would they look to the users.
  - It contains selectors which have many types to help in identfying the elements in which the rules will be applied upon.
  - CSS can be applied in 3 different ways:
     1-Inline styling: which you declare style element inside the HTML element        you would like to design.
	 2-Internal styling: By identyfing the style tag in the head and then you        apply designs by calling each element by it's name or selectors.
	 3-External styling: By defining a separate CSS file and add all designs inside of it then simply call it inside the HTML using the "Link" tag in the head.
- Declrations of the CSS is defined in two parts: the properties of the CSS element and it's value.

  #Now we'll talk about JavaScript & jQuery:
 - JavaScript is series of statements thats executed one after another just like any other programming language also it's very precise.
- Variables store temporary data inside of them that will be useful later on.
- Arrays ae used to store a huge number of related data, makes operations on such a group of information much more efficient and easier.
- JS consists of only three data types, that are strings, booleans and numbers unlike other programming languages.
- Expressions eventually become a single value and they rely on operators to calculate a value. 
### Loops and comparison operators:
In this section we are talking about the most important coding basics you’ll need not only in JS but in almost every programming language as they make the perfect logical sense when you are trying to translate from our human language to the computer language, starting here with:
*** Comparison operators ***:
These operators are used to compare two values and would return the results in the form of ‘True’ or ‘False’ and to evaluate specific segments of the code, and for other different reasons.
## These comparison operators are:

1.	*** Is Equals To ***: It compares two values to check if they are the same.
Syntax: (==).
2.	*** Is Not Equals To ***: It compares two values to check if they are not the same (to sometimes make exceptions).
Syntax: (!=).
3.	*** Strict Equal To ***: It doesn’t only make sure that the values are the same but also the data types.
Syntax: (===).
4.	*** Strict Not Equal To ***: It makes sure that both values and data types are not the same.
Syntax: (!==).
5.	*** Greater than ***: Compares two values and returns the greater value.
Syntax: (>).
6.	*** Less than ***: Compares two values and returns the less great value.
Syntax: (<).
7.	*** Greater than or equal to ***: Checks whether one value is greater than or equals to the other.
Syntax: (>=).
8.	*** Less than or equal to ***: Checks whether one value is less than or equals to the other.
Syntax: (<=).

*** Logical operators***:

These operators allow you to compare two comparison operators like you can actually combine them in one sentence using logical operators.
And we have three logical operators:

1.*** And operator ***: Tests more than one condition and depending on the combination of both results the final result is formatted.
Syntax: (&&). 

2.*** Or operator ***: Tests at least one condition and determines the other then based on that the final result is formatted:
Syntax: (||).

3.*** Not operator ***: Takes one value and gives the opposite of it as a final result.
Syntax: (!).
Contains a condition inside of them if the condition returns true all statements inside of it will run, it will recheck the code after each iteration and execute the statements until the condition returns false only then it will break out.
There are 3 types of loops:
1-For loop.
2-While loop.
3-Do while loop.