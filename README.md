Download Link: https://assignmentchef.com/product/solved-program-that-counts-the-number-of-times-each-ascii-character-code-occurs
<br>
<span style="font-weight: 400;">First you are asked to write a program that performs a basic task (namely counting the number of times each ASCII character code occurs in the standard input, and printing results to standard output). You should do Part 1 and test it carefully to make sure it is working before proceeding to the next step. In the next part you will add features allowing a user to list input files and/or an output fle on the command line.</span>




<ol>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Complete </span><a href="https://www.cs.ucsb.edu/~mikec/cs16/assignments/pa5/counts.cpp"><span style="font-weight: 400;">counts.cpp</span></a><span style="font-weight: 400;"> using the tools provided in </span><a href="https://www.cs.ucsb.edu/~mikec/cs16/assignments/pa5/common.h"><span style="font-weight: 400;">common.h</span></a><span style="font-weight: 400;"> as follows:</span>

  <ul>

   <li style="font-weight: 400;"><span style="font-weight: 400;">Read characters from standard input until </span><span style="font-weight: 400;">EOF</span><span style="font-weight: 400;"> (the end-of-file mark) is read (see the textbook page 353, and know that cin has most of the same features as input file streams. Do not prompt the user to enter text – just read data as soon as the program starts.</span></li>

   <li style="font-weight: 400;"><span style="font-weight: 400;">Keep a running count of each different character encountered in the input, and keep count of the total number of characters input.</span></li>

  </ul></li>

</ol>

<table>

 <tbody>

  <tr>

   <td>

    <ul>

     <li style="list-style-type: none;">

      <ul>

       <li style="font-weight: 400;"><span style="font-weight: 400;">Note there are a total of 128 </span><a href="https://www.cs.ucsb.edu/~mikec/cs16/assignments/pa5/ascii.html"><span style="font-weight: 400;">ASCII codes</span></a><span style="font-weight: 400;">, equal to the value of the symbolic constant NUM defined in common.h. Get familiar with the features of common.h – many of them are handy, and you will be required to use some of them in later steps.</span></li>

      </ul></li>

    </ul></td>

  </tr>

 </tbody>

</table>

<ul>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Print a neat table that shows each different input code, the corresponding character and its count, and print the total count at the end. Do not print any rows for ASCII codes that are not included in the input text.</span></li>

 <li style="font-weight: 400;"><span style="font-weight: 400;">You must </span><i><span style="font-weight: 400;">exactly match</span></i><span style="font-weight: 400;"> the format of our solution’s </span><a href="https://www.cs.ucsb.edu/~mikec/cs16/assignments/pa5/results1.txt"><span style="font-weight: 400;">basic results</span></a><span style="font-weight: 400;">, and so you must use the symbols and functions defined in common.h. Do NOT print anything any other way.</span></li>

</ul>

<ul>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Use </span><span style="font-weight: 400;">prHeader</span><span style="font-weight: 400;"> one time at the start.</span></li>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Use </span><span style="font-weight: 400;">prCountStr</span><span style="font-weight: 400;"> for each row that corresponds to a special character (codes 0-32, and 127), and use the symbol strings provided in common.h.</span></li>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Use </span><span style="font-weight: 400;">prCountChr</span><span style="font-weight: 400;"> for each row that corresponds to a printable character (codes 33-126).</span></li>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Use </span><span style="font-weight: 400;">prTotal</span><span style="font-weight: 400;"> one time at the end.</span></li>

 <li style="font-weight: 400;"><span style="font-weight: 400;">You can test it by typing text manually, in which case you must enter </span><span style="font-weight: 400;">ctrl-D</span><span style="font-weight: 400;"> on Linux (or </span><span style="font-weight: 400;">ctrl-Z</span><span style="font-weight: 400;"> on Windows) to end the input. Or better, test it by redirecting a file using the Linux redirection operator (</span><span style="font-weight: 400;">‘&lt;‘</span><span style="font-weight: 400;">). For example, to input this sample text file named </span><a href="https://www.cs.ucsb.edu/~mikec/cs16/assignments/pa5/sample.txt"><span style="font-weight: 400;">sample.txt</span></a><span style="font-weight: 400;">, in our second sample run, notice that we typed the following:</span></li>

 <li style="font-weight: 400;"><span style="font-weight: 400;">./counts &lt; sample.txt</span></li>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Another good input file for testing is </span><a href="https://www.cs.ucsb.edu/~mikec/cs16/assignments/pa5/allchars.txt"><span style="font-weight: 400;">allchars.txt</span></a><span style="font-weight: 400;"> which contains one of each ASCII character code. Of course, many of these codes don’t show up well when you view it in your web browser, but your program should be able to identify them. Here’s the result (of course): </span><a href="https://www.cs.ucsb.edu/~mikec/cs16/assignments/pa5/allchars-out.txt"><span style="font-weight: 400;">allchars-out.txt</span></a><span style="font-weight: 400;">. A copy of allchars.txt is in ~cs16/pa5/ too.</span></li>

</ul>

<table>

 <tbody>

  <tr>

   <td>

    <ol>

     <li style="font-weight: 400;"><span style="font-weight: 400;">Make a backup copy of counts.cpp before attempting Part 2. A fully working basic version (i.e., just Part 1) will earn half-credit for this project, more points than a broken enhanced version that we cannot test at all.</span></li>

    </ol></td>

  </tr>

 </tbody>

</table>

<ul>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Enhance counts.cpp so that it responds to command line arguments as specified below. Here is an example program showing how command line arguments can be processed: </span><a href="https://www.cs.ucsb.edu/~mikec/cs16/assignments/pa5/args.cpp"><span style="font-weight: 400;">args.cpp</span></a><span style="font-weight: 400;">.</span></li>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Let the user enter input filenames and/or an output filename on the command line.</span>

  <ul>

   <li style="font-weight: 400;"><span style="font-weight: 400;">If any input files are requested, then read from those files instead of cin – count all of the characters in all of the input files as one set of input data.</span></li>

   <li style="font-weight: 400;"><span style="font-weight: 400;">if a command line argument begins with ‘-o’, then the next command line argument is an output filename (</span><span style="font-weight: 400;">-o name</span><span style="font-weight: 400;">). In that case print results to the file instead of cout. Ignore any command line arguments that may follow the output filename.</span></li>

  </ul></li>

 <li style="font-weight: 400;"><span style="font-weight: 400;">Signal errors by using the functions defined at the bottom of common.h:</span>

  <ul>

   <li style="font-weight: 400;"><span style="font-weight: 400;">Use </span><span style="font-weight: 400;">badFile</span><span style="font-weight: 400;"> if a file (whether input or output) cannot be opened.</span></li>

   <li style="font-weight: 400;"><span style="font-weight: 400;">Use </span><span style="font-weight: 400;">badOption</span><span style="font-weight: 400;"> if an argument begins with </span><span style="font-weight: 400;">‘-‘</span><span style="font-weight: 400;"> but the second character is not </span><span style="font-weight: 400;">‘o’</span><span style="font-weight: 400;">.</span></li>

   <li style="font-weight: 400;"><span style="font-weight: 400;">Use </span><span style="font-weight: 400;">missing</span><span style="font-weight: 400;"> if the </span><span style="font-weight: 400;">‘-o’</span><span style="font-weight: 400;"> option is not followed by a filename (even if the user types </span><span style="font-weight: 400;">-oname</span><span style="font-weight: 400;"> with no space before the name).</span></li>

   <li style="font-weight: 400;"><span style="font-weight: 400;">Match these </span><a href="https://www.cs.ucsb.edu/~mikec/cs16/assignments/pa5/results2.txt"><span style="font-weight: 400;">enhanced results</span></a><span style="font-weight: 400;">. Notice the last several runs show error messages and no results.</span></li>

  </ul></li>

</ul>