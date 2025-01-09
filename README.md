# DNA_transcribe_translate
A jupyter notebook to transcribe and translate a DNA sequence to produce a protein sequence.


## Python and Bioinformatics Activity
Now that you have learned about protein synthesis and bioinformatics, we’re going to learn how 
to write code to do this pathway for us almost instantly! Scientists use bioinformatics because it 
would take too long to analyze genetic information by hand. Genes can be millions of base pairs 
long so it would be almost impossible for anyone to analyze them by hand! Today we will learn 
how to transcribe and translate DNA using Python, one of the most widely used programming 
languages as well as one of the most common languages used in Bioinformatics! Your first step 
will be to start a new Python script.
1. Navigate to https://jupyter.org/try-jupyter/lab/
2. Scroll down and click the “Python (Pyodide)” icon → <br />
a. Now you’re ready to start programming!
3. First, let’s practice making some variables and calling a function! <br />
a. To create a new variable, type a variable name and the equal sign, let’s call this first 
variable hello to keep it simple. Make sure there are no spaces in your variable 
name. <br />
b. Now, add an equal sign to tell Python what your variable is. <br />
c. Next, let’s make this variable equal to a string, “hello world” <br />
d. Your variable should now look like this: hello = “hello world” <br />
4. Now let’s call a function to print this variable. For this, we will use the “print” function. <br />
a. In a new line, type print() to call the print function. <br />
b. You will need to tell it to print your variable, so within the parenthesis type the 
name of your variable <br />
c. Your file should now look like this → <br />
5. Next, click the run arrow at the top of the 
screen 
6. A new line should pop up now displaying your “hello world” string! You’ve just written 
your first line of code!
7. Now that we know how to call functions, it’s time to write our own function! We do this 
by defining (def) a function! <br />
a. Functions are written as def function_name(arguments): <br />
b. These are usually named in a way that explains what the function does, so let’s 
name our function “transcribe” <br />
c. The only argument we’ll need for this function is the DNA sequence, so we can call 
this part of the function “DNA” <br />
d. Your page should now look like this: <br />
e. Now that we’ve defined our function, we have to tell it what to do! <br />
8. To start out, we will need to create a dictionary that tells us which bases become which 
other bases during transcription (this step changes DNA to mRNA). Review your 
transcription notes to help you! <br />
a. First, tell me which bases become what during transcription: <br />
A → __U__ <br />
T → _____ <br />
C → _____ <br />
G → _____ <br />
b. Next, we must turn this into a format Python can understand. We do this by using a 
dictionary! These work the same way a real dictionary works, by stating a “word” 
and then stating a “definition” to that word! In Python, these are created using curly 
brackets. <br />
c. To create our dictionary variable, we must first name it. I’d recommend naming it 
something that makes sense such as DNA_to_RNA. Then we add our equal sign! <br />
d. Now we will create our “words” and definitions! In Python, it looks like this: 
dictionary_name = {“word”: “definition”, “word_2”: “definition_2”} <br />
e. I’ll get you started on your dictionary here, just fill in the blanks! <br />
DNA_to_RNA = {“A”: “U”, “T”: “___”, “C”: “___”, “G”: “___” <br />
f. Now add this dictionary to your Python file! <br />
9. The last thing we will need to define before writing the functional part of the code is to 
create a variable for our RNA sequence to be stored in. For this, we will create an empty 
string or a string that has no text between the quotations. Your variable should look like 
this: <br />
RNA = “” <br />
10. Now, your code should look like this overall:
11. Now here’s where the code gets interesting! To have the code go through our DNA strand, 
we will use a “for” loop. This basically means that it will do something for every base in 
the DNA strand. In our case, for every base in the DNA strand, it will replace it with the 
“definition” to create our RNA strand!
12. Our for loop will be written like this which basically says 
“do something for every base in the DNA” → <br />
a. Notice the colon at the end. This means we will need to indent the next line <br />
13. Next, we will tell the for loop what to do at every base. What we want it to do at every base 
is to get the “definition” of that base from our dictionary and then assemble a new RNA 
strand. We do this with the “get” function which makes the code much simpler! <br />
a. The get function is written in a unique way which looks like this: <br />
variable_name.get(what you want it to get) <br />
b. In plain English, this means “from the variable name (in our case, the dictionary), 
get what you want it to get” <br />
c. Try to write out what we want to get here! <br />
_____________________.get (________________________) <br />
 Dictionary Name Variable we want to get (hint, this is what we get out 
of the “for” loop! <br />
d. Next, we want to add this to our new RNA strand! We do this with the += operation.
i. This will look like RNA += DNA_to_RNA.get(base) <br />
14. The last step is to tell it to return your completed RNA strand! <br />
a. The return function is very simple and is written like this:
return variable_name
15. Now that everything is written, your code should look like this:
16. Congratulations, you’ve just written your first function!!! Now all we need to do is run it!
17. Bellow your function, define a DNA string. You can use any valid DNA sequence:
a. DNA = “ATCGGATACA”
18. Next, let’s make a new RNA strand. Define an RNA variable and set it equal to your 
transcription function with DNA as the argument. This sends your DNA strand through 
your new function: <br />
a. RNA = transcribe(DNA) <br />
19. Finally, print your new RNA strand with the print function! <br />
a. print(RNA) <br />
20. Now that your code is done, the last step is to hit the run button! 
21. Now that you’ve written your code, try it out on a few different DNA sequences! Just 
change the DNA sequence and rerun your code! 
DNA Sequence mRNA Sequence
CATCATCAT
TAC
ATCGAA
 Here’s your new RNA strand!!
