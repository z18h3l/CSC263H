java c
Computer Science CSC263H 
September 4, 2024 
Homework Assignment #1 
Due: September 11, 2024, by 11:00 am 
• You must submit your assignment through the  Crowdmark system. You will receive by email an invitation through which you can submit your work. If you haven’t used Crowdmark before, give yourself plenty of time to figure it out! 
• You must submit a separate PDF document with for each question of the assignment. 
• To work with one or two partners, you and your partner(s) must form a group on Crowdmark (one submission only per group).  We allow groups of up  to  three students.  Submissions by groups of more than three students will not be graded. 
• The PDF file that you submit for each question must be typeset (not handwritten) and clearly legible. To this end, we encourage you to learn and use the LATEX typesetting system, which is designed to produce high-quality documents that contain mathematical notation. You can use other typesetting systems if you prefer, but handwritten documents are not accepted. 
• If this assignment is submitted by a group of two or three students, for each assignment question the PDF file that you submit should contain: 
1. The name(s) of the student(s) who wrote the solution to this question, and 
2. The name(s) of the student(s) who read this solution to verify its clarity and correctness. 
• By virtue of submitting this assignment you (and your partners, if you have any) acknowledge that you are aware of the homework collaboration policy for this course, as stated here . 
•  For any question, you may use data structures and algorithms previously described in class, or in prerequisites of this course, without describing them. You may also use any result that we covered in class (in lectures or tutorials) by referring to it. 
• Unless we explicitly state otherwise, you should justify your answers. Your paper will be marked based on the correctness and efficiency of your answers, and the clarity, precision, and conciseness of your presentation. 
• The total length of your pdf submission should be no more than 3 pages long in a 11pt font. 
Question 1. (20 marks)  The following procedure has an input array A[1..n] with n ≥ 2 arbitrary integers.
In the pseudo-code, “return” means immediately exit the procedure and then halt. Note that the indices of array A starts at 1.
weirdo(A[1..n])
1   n = A. size
2 for i = 1 to n                           // i = 1, 2, . . . , n
3 for j = 1 to n                    // j = 1, 2, . . . , n
4 if A[n - j + 1]  j then return 
5 if (A[i]  n - i + 1) or (A[1] + A[2] = 2n - 1) then return 
6 return 
Assume that each assignment, comparison, and arithmetic operation takes constant time.
Let T(n) be the worst-case time complexity of calling weirdo(A[1..n]) on an array A of size n ≥ 2. Give a function f(n) such that T(n) is Θ(f(n)).
Justify your answer by explaining why it is O(f(n)), and why it is Ω(f(n)). Any answer without a sound and clear justification may receive no credit.
Question 2. (20 marks)We want to compute the median of every prefix  of an  input array A[1..n] of arbitrary integers.   More precisely, design an algorithm that outputs another array M[1..n], so that M[i] is equal to the median of the integers in the subarray A[1..i]. Recall that when i is odd, the median of A[1..i] is the element of rank (i+1)/2 in the subarray, and when i is even, the median is the average of the elements with ranks i/2 a代 写CSC263H Data Structures and Analysis September 4, 2024 Homework Assignment #1
代做程序编程语言nd i/2 + 1. Your algorithm should run in worst-case time O(nlog n).Hint: Maintain two heaps for the subarray A[1..i]:  one that contains「i/2l elements of this subarray, and one that contains  li/2」elements of this subarray. What elements of A[1..i] should each one of these heaps contain?  What kind of heap each one them is?  How do you use them to compute the median of A[1..i]? How do you maintain these heaps when you increase i to i + 1?
a. Describe your algorithm in clear and concise English, and also provide the corresponding pseudocode. Argue that your algorithm is correct.
b. Justify why your algorithm runs in time O(nlog n) in the worst case.
[The questions below will not be corrected/graded.  They are given here as interesting problems that use material that you learned in class.]Question 3. (0 marks)   Design an efficient algorithm for the following problem.  The algorithm is given an integer m ≥ 1, and then a (possibly infinite) sequence of distinct integer keys are input to the algorithm, one at a time. A print operation input can also occur at any point between keys in the input sequence. When the algorithm gets a print operation input, it must print (in any order) the m smallest keys among all the keys that were input before this print.
For example, suppose m = 3, and the keys and print operations are successively input to the algorithm in the following order:
18, 13, 29, 4, 11, 22, print, 8, 15, 7, 14, 3, 9, 12, print, 2, 5, . . .The first print should print 13, 4, 11 (in any order), and the second print should print 4, 7, 3 (in any order). Assume that:  (1) m does not change during an execution of the algorithm,  and  (2) at least m keys are  successively input to the algorithm before the algorithm gets its first print input.
Describe a simple algorithm that solves the above problem with the following worst-case time complexity:
•  O(log m) to process each key input.
• O(m) to perform. each print operation.
Your algorithm must use a data structure that we learned in class. 
•  State which data structure you are using and describe the items that it contains.
• Explain how your algorithm processes a key input, and how it processes a print operation input. First describe this clearly and concisely in English, and then give the pseudo code.
• Explain why your algorithm achieves the required worst-case time complexity described above.
• Prove that your algorithm is correct (Hint: use induction. What is your induction hypothesis?)Question 4. (0 marks)   Let A be an array containing n integers.  Section 6.3 of our textbook  (CLRS) describes a procedure, called Build-Max-Heap(A), that transforms array A into a max-heap in O(n) time. That procedure works “bottom-up”, using Max-Heapify repeatedly.
Another way of transforming A into a max-heap is to insert the elements of A into the heap one at a time. Specifically, the algorithm is as follows:
Build-by-Inserts(A)
A.heapsize := 1
for i := 2..n do 
Max-Heap-Insert(A, A[i])
a. Give an example of an input array A for which the two procedures Build-Max-Heap and Build- by-Inserts produce different outputs. Keep your example as small as possible.b. Let T(n) be the worst-case time complexity of Build-by-Inserts for an input array A of size n. Prove that T(n) is Θ(nlog n).  (Recall that the worst-case time complexity of Build-Max-Heap is O(n), and therefore Build-Max-Heap is more efficient than Build-by-Inserts.)

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
