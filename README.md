Download Link: https://assignmentchef.com/product/solved-comp-206-mini-assignment-2-solution
<br>
<h2><u>Command-line Bash Script</u></h2>




Create a script called <strong>MakeProject.sh</strong> that will be used by you to automate the process of creating well formed software development directories.




This bash script will be used at the command-line as follows: <strong>./MakeProject.sh name</strong> Where <strong>name</strong> is provided by the user at the command-line and is the project name.  The project name must be a single word (it cannot have spaces or other white characters).




The script will do the following in this order:




<ul>

 <li>Using absolute path the script changes directory to your home directory.</li>

 <li>Next it verifies whether a subdirectory called <strong>project</strong> If it does not exist it creates that directory.</li>

 <li>Next it changes directory moving into the project subdirectory using relative path.</li>

 <li>Next it verifies whether a subdirectory called <strong>cs206</strong> If it does not exist it creates that directory.</li>

 <li>Next it changes directory moving into the cs206 subdirectory using relative path.</li>

 <li>Next it verifies whether a subdirectory called <strong>name</strong> (ie. The word the user provided at the command-line) exists.

  <ul>

   <li>If it <strong>does</strong> exist then the script terminates with an error message: “This project name has already been used.”.</li>

   <li>If it <strong>does not</strong> exit, it then creates the subdirectory and below that directory it creates the following additional subdirectories within the project directory: <strong>archive</strong>, <strong>backup</strong>, <strong>docs</strong>, <strong>assets</strong>, <strong>database</strong>, and <strong>source</strong>.</li>

  </ul></li>

 <li>Next it changes directory moving into the source subdirectory using relative path.</li>

 <li>Finally, the bash script generates (does not copy from another location) a Bash script file called <strong>sh</strong> and this script file simply copies all the files with the file extension .c and .h into the backup directory using relative paths. The user would run this script from within the source directory by typing: <strong>./backup.sh</strong> • The script terminates by displaying: “You project directories have been created.”</li>

</ul>
















Vybihal           Page 1 of 2      9-22-2017 McGill University             COMP 206      School of Computer Science

<h2>WHAT TO HAND IN</h2>

Everything must be submitted to My Courses before the due date. Remember that you can hand in your assignment up to two days late but there will be a penalty of 5% each day. After that, your assignment will not be accepted.  Please hand in the following:

<ul>

 <li>A single Bash script called MakeProject.sh</li>

</ul>

<strong> </strong>

<h2>HOW IT WILL BE GRADED</h2>

The assignment is worth a total of 20 points.

<ul>

 <li>4 points – Changing directories o 5 points – Testing existence of directories o 4 points – Creating directories o      2 points – Displaying error messages</li>

 <li>5 points – Creating the backup.sh script programmatically</li>

</ul>

<strong> </strong>

<h2>GRADING RULES</h2>

The following rules are followed by the TA when grading assignments:

<ul>

 <li>A program must run in order to get a grade (even if it does not run well). If it does not run (does not compile) it will receive a zero. (Make sure to run your programs from Trottier – they sometimes do not run the same from home when logging in using putty.)</li>

 <li>The TA will grade using the linux.cs.mcgill.ca server.</li>

 <li>All questions are graded proportionally (assuming the program runs at all). This means that if 40% of the question is correct, you will receive 40% of the grade.</li>

</ul>

Vybihal                                                  Page 2 of 2                                              9-22-2017