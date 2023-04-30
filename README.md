Download Link: https://assignmentchef.com/product/solved-ensf614-lab-4
<br>
<strong>Notes: </strong>

<ul>

 <li>In this lab also you can work with a partner.</li>

 <li>This is another important lab assignment, and it is aimed to help you understanding very essential topics such as dynamic allocation of memory in C++, and concepts such as copying objects in C++.</li>

 <li>Material on exercises B and C will be discussed during the lecture on Oct 13 and 15.</li>

</ul>

<strong> </strong>

<strong>Exercise A: Design a Dynamic Array Class </strong>




<strong>Read This First: </strong>

<strong> </strong>

This exercise is designed to give you some insight about a resizable array class. It also shows other feature of C++ including proper way of copying objects of this class.

<strong> </strong>

<strong>What to do: </strong>

<strong> </strong>

Download files in the files MyArray.h and lab4ExA.cpp. Then read the file MyArray.h, which tells you what the MyArray class interface is and what the member variables are. Pay close attention to the comment that describes the memory management strategy for the MyArray class.

Read the file lab4ExA.cpp, which demonstrates how a MyArray object could be used.  The file MyArray.cpp is missing. It’s your job to write this file.

<strong> </strong>

<strong>What to Submit: </strong>

<strong> </strong>

Submit your file MyArray.cppand your program output as part of your lab report

<strong> </strong>

<strong>Exercise B: Using C++ library classes,</strong> vector <strong>and </strong>string

The objective of this exercise is to gain some experience in understanding the C++ library classes, vector, and string.

<strong>What to Do: </strong>




Download the files lab4ExB.cpp from D2L.  In this file there is a declaration of vector &lt;string&gt;.  If you compile and run this program it creates the following output:

ABCD

EFGH

IJKL

MNOP

QRST

1

Let’s visualize this output as a matrix of letters (5 rows and 4 columns):

<table width="113">

 <tbody>

  <tr>

   <td width="27">A</td>

   <td width="29">B</td>

   <td width="28">C</td>

   <td width="28">D</td>

  </tr>

  <tr>

   <td width="27">E</td>

   <td width="29">F</td>

   <td width="28">G</td>

   <td width="28">H</td>

  </tr>

  <tr>

   <td width="27">I</td>

   <td width="29">J</td>

   <td width="28">K</td>

   <td width="28">L</td>

  </tr>

  <tr>

   <td width="27">M</td>

   <td width="29">N</td>

   <td width="28">O</td>

   <td width="28">P</td>

  </tr>

  <tr>

   <td width="27">Q</td>

   <td width="29">R</td>

   <td width="28">S</td>

   <td width="28">T</td>

  </tr>

 </tbody>

</table>

Your job is to complete the definition of the function called transpose that creates a new object of vector&lt;string&gt; where its strings are the transpose of the original vector:

<table width="138">

 <tbody>

  <tr>

   <td width="24">A</td>

   <td width="28">E</td>

   <td width="28">I</td>

   <td width="28">M</td>

   <td width="28">Q</td>

  </tr>

  <tr>

   <td width="24">B</td>

   <td width="28">F</td>

   <td width="28">J</td>

   <td width="28">N</td>

   <td width="28">R</td>

  </tr>

  <tr>

   <td width="24">C</td>

   <td width="28">G</td>

   <td width="28">K</td>

   <td width="28">O</td>

   <td width="28">S</td>

  </tr>

  <tr>

   <td width="24">D</td>

   <td width="28">H</td>

   <td width="28">L</td>

   <td width="28">P</td>

   <td width="28">T</td>

  </tr>

 </tbody>

</table>

To test your program, you can change the values of the constants ROWS and COLS, in the main function to make sure your function works with other sizes of the String_Vector.

<strong>What to Submit: </strong>

Submit the definition of your function transpose and the program’s output.

<strong>Exercise C: C++ File I/O </strong>

The objective of this exercise is to help you understanding the basics of file I/O in C++.




<strong>What to Do: </strong>




Download the files lab4ExC.cpp from D2L. If you read this file carefully you will realize that this simple C++ program creates a binary file (for example: cities.bin), that contain several records of type struct City.

Each record has two double types represent x and y coordinates of a city on Cartesian Plan, followed by the name of the city, which is stored as a C-string in an array of characters with 30 elements. The program has several functions, the implementation of one of them, called print_from_binary, is missing. Your task will be to write the definition of the missing function. This function is supposed to read the content of the binary file created by the program, and display the its content (records both on the screen and into a text file, using in the following format:

Name: Calgary, x coordinate: 100, y coordinate: 50




Here is the functions prototype and interface comment:

void print_from_binary(char* filename);

/* PROMISES: uses ifstream library object to open the binary file named

<ul>

 <li>“filename”, reads the content of the file which are objects of struct City</li>

 <li>(one record at a time), and displays them on the screen. It also saves the records</li>

 <li>into a text-file that its name must be filename argument, but with the extension of .txt</li>

</ul>

*/

<strong>What to Submit: </strong>

Submit the definition of your function print_from_binary and the content or the generated text file, as part of your lab report in PDF format.

<strong> </strong>