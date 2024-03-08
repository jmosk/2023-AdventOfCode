The purpose of these solutions is NOT to create the most efficient and complex one-line
solutions to each puzzle but to provide a detailed solution along with an explanation of each
of the steps taken to get the correct answer. Not being an advanced and skilled APL programmer
I can see my solutions are not taking advantage of the power of various primitives. But,
they do derive the correct solution to the puzzles solved. My knowledge of APL is mostly
the old traditional one. I learned APL on an IBM\1130 50+ years ago and read Ken Iverson's
book back then. So I am not very up to speed on all the new functions Dyalog has added to 
the language and their power. I still have my IBM Selectric Typewriter type ball with APL
characters on it that I used on the 1130. 

This set of solutions does not show the most efficient way of doing things in APL.
One of the nice features of APL is performing things in parallel. Looking over
solutions presented by others in the APL AoC Wiki, I can see where some of the
operations implemented could potentially be done simultaneously. For example,
Day 3 part 2, found which special characters needed to be examined to derive the
solution, but then extracted the solution for each special character one at a time. 
These could have all been put in a single array and executed together instead of
processing the same function for each special character. It is best to think
differently in APL regarding what can be done in parallel, instead of doing
sequentially. As an aside, at least in one case, I found that when I tried to
execute a posted solution with the test data, it did not produce the correct result.

First, the general way of approaching the solution is discussed. Then there is a
step-by-step breakdown of how the solution is implemented. The apl##_trace version
displays the output from each function performed along the way to the solution
so the reader can follow along and understand what each step is doing and how
the primitives are deriving the data shown.

This is a slow work in progress as I have time to work on the 2023 puzzles. But I thought
it could be of interest to have fully documented solutions to the puzzles. 

Code to solve AoC puzzles are of the form:<br>
<li> apl#a - for part 1
<li> apl#b - for part 2 - But part 2 is sometimes in the same file as part 1<br>
</li>
<br>
<p style="margin-left::200px; ">
  Note:<br>
  Starting with apl4a, the trace function has been built into the APL source
  code. At the top of the program is 'db' which is set to 1 to provide debug
  or trace output. The APL function in this directory called trace implements
  the optional display of data. The variable called 'test' is set to 1 to use
  the game test data or set to 0 to use the game data. And there might be other
  variables that can be set to operate different algorithms implemented. 
</p>
<br>Verification of sample data is:
<li>  apl#a_trace - with results of each step displayed
<li>  apl#b_trace
<br><br>Data is:
<li>  test#a.txt - sample data
<li>test#b.txt
<li> data#a.txt - AoC data to process
<li>data#b.txt - oftentimes data#a.txt is used for both parts
</li>
  
