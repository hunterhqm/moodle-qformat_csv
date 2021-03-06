NEW in 3.6

# Description
Question formats import plugin 

==============================

This plugin contains support for importing multichoice and truefalse questions in CSV format file in question bank.
The CSV format is a very simple way of creating questions using a CSV(Comma separated value) file.You can edit a lot of questions in Excel or in WPS table,then save the file in CSV format.PS,if the language is not english,you may open the file with  the app like notepad to change the coding to UTF-8.
The first line of the CSV file must contain the headers separated with commas
===============================

# Multichoice questions format
The multichoice questions CSV file used for import should have the following structure :
-A CSV file with all questions in comma separated value form with a .csv extension
-The first line contains the headers separated with commas for example:
 multichoicename,questiontext,choices,answer,generalfeedback,defaultmark,qtype
-Next lines contain the details of the question,
  each of the line contain question name, question text, choices(semicolon ';' separated value), and
  answers,generalfeedback,defaultmark,qtype(multichoice or single),all separated by commas.
-Each line contains all the details regarding the one question ie. question name, question text, options, and answer.
-You can also download the multichoice sample CSV(sampleMultichoice.csv) file for your reference.

# truefalse questions format
The truefalse questions CSV file used for import should have the following structure :
-A CSV file with all questions in comma separated value form with a .csv extension,UTF-8 coding
-The first line contains the headers separated with commas for example:
 truefalsename,questiontext,answer,generalfeedback,defaultmark
-Next lines contain the details of the question,
  each of the line contain question name, question text,answer（true or false，1 or 0）,generalfeedback,defaultmark,all separated by commas.
-You can also download the truefalse sample CSV(sampleTruefalse.csv) file for your reference.




=============================================================================================================================
IMPORTANT NOTES:

* You have to save the file strictly in csv format. Don't save it as an Excel document or anything like that.
* Non-ASCII characters like 'quotes' can cause import errors.
* To avoid this, always save your text file in UTF-8 format (most text editors, even libre office, will ask you).
* The Header must be as it is shown in the example everything is case sensitive as shown below otherwise, the import will fail.

* If you want to have comma(,) between the text may be in question text or in options text then
you must include that text between the double quotes(") like below in the 2nd question, where entire
question text is included between the double quotes like this "3, 4, 7, 8, 11, 12, ... What number should come next?"

 multichoicename,questiontext,choices,answer,generalfeedback,defaultmark,qtype
 Question1,can you choose all the right answers?, A is ok;B is wrong ;C is ok;D is ok, ACD,right answers are ACD,2,multichosce
 Question2,"3, 4, 7, 8, 11, 12, ... What number should come next?", 7;10;14;15, D,right answers is D,1,single




* Please, see the sample csv files for more clarification.
* Questions imported in question bank can also be imported when creating a quiz from the question bank.
