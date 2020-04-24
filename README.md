# Horse-Problem
A. Project purpose
In this project, we have a horse stay on the square(1,1). We want to find the way such that the horse visits all 64 squares without any repetion

B. Solution
At the beginning, we need to mark the square(1,1) with 1 and all the remaining squares with 0. From the square (i,j), we have total 8 directions that the horse can go. We can go to the square (i-1,j-2),(i-2,j-1),(i-2,j+1),(i-1,j+2),(i+1,j+2),(i+2,j+1),(i+2,j-1),(i+1,j-2).
When we move to another square marked with 0, we have to mark this square with 1 to ensure there will be no repetition in our movement. In particular, we just move to a square which is marked with 0 in our movement and cannot move to a square marked with 1. After each movement, we will increase our step by 1. Finally, when our step is 64, we will print the way how we finish it.

C. Recursive Method(Explaining in my code)
