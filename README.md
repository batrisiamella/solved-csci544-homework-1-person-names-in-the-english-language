Download Link: https://assignmentchef.com/product/solved-csci544-homework-1-person-names-in-the-english-language
<br>
Person names in the English language typically consist of one or more forenames followed by one or more surnames

(optionally preceded by zero or more titles and followed by zero or more suffixes). This situation can create ambiguity, as it is often unclear whether a particular name is a forename or a surname. For example, given the sequence <em>Imogen and Andrew Lloyd Webber</em>, it is not possible to tell what the full name of Imogen is, since that <a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber">would depend on whether </a><a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber"><em>Lloyd</em></a><a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber"> is part of Andrew’s forename or surname (as it turns out, it is a surname: </a><a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber">Imo</a><a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber">g</a><a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber">en Llo</a><a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber">y</a><a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber">d Webber</a><a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber"> is the daughter of</a> <a href="https://en.wikipedia.org/wiki/Andrew_Lloyd_Webber">Andrew Llo</a><a href="https://en.wikipedia.org/wiki/Andrew_Lloyd_Webber">y</a><a href="https://en.wikipedia.org/wiki/Andrew_Lloyd_Webber">d Webber</a><a href="https://en.wikipedia.org/wiki/Imogen_Lloyd_Webber">). This exercise explores ways of dealing with this kind of </a>ambiguity.

You will write a program that takes a string representing the names of two persons (joined by <em>and</em>), and tries to predict the full name of the first person in the string. To develop your program, you will be given a set of names with correct solutions: these are not names of real people – rather, they have been constructed based on lists of common forenames and surnames. The names before the <em>and</em> are the first person’s forenames, any titles they may have, and possibly surnames; the names after the <em>and</em> are the second person’s full name. For each entry, your program will output its best guess as to the first person’s full name. The assignment will be graded based on accuracy, that is the number of names predicted correctly on an unseen dataset constructed the same way.

Data

A set of development and test data is available as a compressed ZIP archive on <a href="http://blackboard.usc.edu/">Blackboard</a><a href="http://blackboard.usc.edu/">.</a> The uncompressed archive contains the following files:

A test file with a list of conjoined names.

A key file with the same list of conjoined names, and the correct full name of the first person for each example.

Readme and license files, which will not be used for the exercise, but may contain useful information.

The submission script will run your program on the test file and compare the output to the key file. The grading script will do the same, but on a different pair of test and key files which you have not seen before.

Program

You will write a program called full-name-predictor.py in Python 3 (Python 2 has been deprecated), which will take the path to the test file as a command-line argument. Your program will be invoked in the following way:

&gt; python full-name-predictor.py /path/to/test/data

The program will read the test data, and write its answers to a file called full-name-output.csv. The output file must be in the same format of the key file.

All submissions will be completed through <a href="https://labs.vocareum.com/main/main.php">Vocareum</a><a href="https://labs.vocareum.com/main/main.php">;</a> please consult the <a href="http://ron.artstein.org/csci544-2020-08/Student-Help-Vocareum.pdf">instructions for how to use Vocareum</a>.

Multiple submissions are allowed; only the final submission will be graded. Each time you submit, a submission script is invoked, which runs the program on the test data. Do not include the data in your submission: the submission script reads the data from a central directory, not from your personal directory. You should only upload your program file to Vocareum, that is full-name-predictor.py; if your program uses auxiliary files (for example, lists of common names), then you must also include these in your personal directory.

You are encouraged to submit early and often in order to iron out any problems, especially issues with the format of the final output.

The output of your program will be graded automatically; failure to format your output correctly may result in very low scores, which will not be changed.

For full credit, make sure to submit your assignment well before the deadline. The time of submission recorded by the system is the time used for determining late penalties. If your submission is received late, whatever the reason (including equipment failure and network latencies or outages), it will incur a late penalty.