# JEE Allocation
____
JEE Seat Allocation Problem states that given N students and N Seats of different Colleges, where each Student has an AIR rank and Category rank. Each Student has a preference Order of Colleges.</br>
Algorithms task is to find the right College for individual Student by comparing individual’s Rank and preference Order of all the Students.
____

#### Approach  :
Consider the following example. </br>
Candidate 1 and Candidate 2 having rank 1 and rank 2 have the best ranks, they can easily get colleges of their first choice (5,4,2,3,1) and (4,5,1,2,3) respectively.
So their Seat allotted would be in College 5 and College 4 respectively.

</br>

* Here, rank and category of the Student can be generated randomly.So the only input we need to take is the preference order of that Student.The Actual seat allocation part will be filled by 40%GEN, 30%OBC, 20%SC and 10%ST.

* Following this we have made use of Gale-Shapley's Stable Marriage Algorithm (O(n2) 
) wherein “Student’s preference order” role is played by Man and “College Seat” role is played by women.
