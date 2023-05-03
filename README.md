Download Link: https://assignmentchef.com/product/solved-cs1331-homework-0-java-development-kit-installation
<br>
This assignment gets you started with the basic tools you will need to complete all of your homework projects. This project will:

<ul>

 <li>Ensure that you have correctly installed the JDK (Java Development Kit)</li>

 <li>Give you practice using a text editor to write Java programs</li>

 <li>Give you practice compiling and running Java programs</li>

 <li>Give you practice identifying and locating an error</li>

 <li>Show you a bit of command line fun</li>

</ul>

<h2>Problem Description</h2>

You are a CS 1331 student who needs to install the JDK, configure it for command line use, and learn how to use a programmer’s text editor to create and edit Java source code.

Please note what is happening here:

&gt; redirects the standard output of a program. 2&gt; redirects stderr, which is used for diagnostics (such as version strings). The first line creates the hw0-output.txt file, and the second line (with the extra &gt;) adds more text to the file. Here is a <a href="http://www.jstorimer.com/blogs/workingwithcode/7766119-when-to-use-stderr-instead-of-stdout">nice discussion</a> of the file descriptors stdin, stdout and stderr.

What this means is that &gt; (or 2&gt;) will overwrite the file, so if you go back to repeat the first step, you’ll need to repeat all the other steps as well.

<h3>Your First Java Program</h3>

<ol>

 <li>Open your text editor and create a file in your newly created hw0 directory named java and enter the following Java program:</li>

</ol>

2.   public class NimblyBimbly {3.       public static void main(String[] args) {4.           for (int i = 0; i &lt; 9; i++) {5.               System.out.print(“u004Du0065u006Fu0077 “);6.           }7.           System.out.println(“…”);8.           System.out.println(“u004Du0065u006Fu0077u0021”);9.       }10. }

<ol start="11">

 <li>On the command line, go to the directory containing your newly created java file and enter javac NimblyBimbly.java. Do a directory listing using the command ls on Mac and Linux or dir on Windows; you should see a file called NimblyBimbly.class that contains the compiled bytecode of your NimblyBimbly program. These commands should look like this:</li>

</ol>

12. Mac / Linux:13. 14. $ javac NimblyBimbly.java15. $ ls16. NimblyBimbly.class NimblyBimbly.java hw0-output.txt …17. 18. Windows:19. 20. C:…cs1331hw0&gt; javac NimblyBimbly.java21. C:…cs1331hw0&gt; dir22. NimblyBimbly.class NimblyBimbly.java hw0-output.txt …

<ol>

 <li>Now enter java NimblyBimbly to run the program and see its output on the command line.</li>

</ol>

<ol start="24">

 <li>Add the output of your program to hw0-output.txt by running</li>

</ol>

25.   java NimblyBimbly &gt;&gt; hw0-output.txt

<ol>

 <li>We have provided a file (Schools.java) for you that contains some sort of error.</li>

 <li>Attempt to compile and run Schools.java (using javac and java).</li>

 <li>At some point during this process you will encounter an error. Read this error carefully and determine where in Schools.java the error originated. That is, identify which line caused the error. It’s alright if you don’t understand what the error means or how to fix it, but do your best to reason through it and think about it. You will encounter lots of errors as you work through homework for this class, so it’s important that you learn early how to decipher the error messages.</li>

 <li>Finally, report your findings. Open up the hw0-output.txt file from before in your text editor. At the bottom, add two lines.

  <ol>

   <li>The first line should say when the error occurred – that is, during compilation or during running.</li>

   <li>On the second line, first put the number of the line causing the error. Then, copy the line itself.</li>

  </ol></li>

</ol>

For example, if you compiled the program successfully, the error happened when you ran it, and line 2 caused the error, you would add

runtime    2. public static void main(String[] args) {

to the file. Be sure to follow the instructions – no extra blank lines, capitalization (or lack of capitalization) as modeled above, etc. Get used to being pedantic about instructions. Computers are nitpicky.