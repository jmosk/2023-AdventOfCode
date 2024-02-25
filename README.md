The purpose of these solutions is NOT to create the most efficient and complex one-line
solutions to each puzzle but to provide a detailed solution along with an explanation of each
of the steps taken to get the correct answer. After I have solved each puzzle I look at
solutions posted by other APL users and learn of the use of other primitives to perform
various functions. That allows me to use some of these other primitives in future solutions.
For example. "selective replacement" was not understood in the day 1 solution and was later 
integrated after a solution was found using other methodologies. Then on day 2, selective
replacement was used to replace spaces inside a matrix with 0's so a row-wise addition
could be used. 

This set of solutions might be of interest to new APL users. First, the general way of
approaching the solution is discussed. Then there is a step-by-step breakdown of how
the solution is implemented. The apl##_trace version displays the output from each
function performed along the way to the solution so the reader can follow along
and understand what each step is doing and how the primitives are deriving the data
shown.

This is a slow work in progress as I have time to work on the 2023 puzzles. But I thought
it could be of interest to have fully documented solutions to the puzzles. 

Code to solve AoC puzzles are of the form:<br>
  apl#a - for part 1
  apl1b - for part 2 - But part 2 is sometimes in the same file as part 1
Verification of sample data is:
  apl#a_trace - with results of each step displayed
  apl#b_trace
Data is:
  test#a.txt - sample data
  test#b.txt
  data#a.txt - AoC data to process
  data#b.txt
  
