java c
Maths 162: Computational Mathematics
Assignment 2, due 7:00pm on September 27th 2024
This assignment is to be submitted online through canvas as a single PDF file, containing answers for all questions, your workings, any figures, and code in a sensible order.
Do not use your phone to take a photo of your computer screen. Photographs of computer screens will not be marked. When handing in code, either copy paste your code into your docu-ment (perhaps with a special coding font), or take a printscreen of your matlab window.
Note that questions are not ordered by difficulty. If question 1 seems hard, don’t assume that the other questions will be harder, they will just be different.
For each question, work through as far as you can - even if you cannot get a complete/perfect answer, write what you can. As the main idea is to demonstrate your understanding of the ideas, methods and programming, do include all your working and your MATLAB code along with the answers that you get from your MATLAB code.
Full marks: 35 marks.
Getting help:
• No cheating. You are allowed to discuss with others how to go about a question, but you must produce your own computations and write your answers by yourself. Copying answers, either from other students, the internet or ’online tutors’ is considered plagiarism.
• Course material: The course book, your notes from lectures, and the tutorials all provide helpful information for answering the assignment questions. There is also the Coder’s guide to programming and the Spider’s guide to Cobwebs.
• Help files in MATLAB: One way to find information about a particular MATLAB function is to type help in the MATLAB Command Window followed by the name of the function. For example, to get help with using sqrt , the square root function, type help sqrt . This gives basic information. For more information, you can click on the link to the Help browser (i.e., the question mark at the top of the MATLAB window.)
• Office Hours: Alastair’s office hours are currently 1:30-3:30 on Thursday. Additional office hours will be available during assignment weeks (These will be announced on Canvas)
1 Diffie-Hellman and Modular inverses (11 marks)
What this question is checking? Modular arithmetic, inverses and key exchange are central to modern cryptography and our ability to communicate securely on the internet. In this question you will test your understanding of Diffie-Hellman key exchange.
The question will mainly focus on methods you have seen in class (all be it, computationally difficult ones).
Now to the question...
(a) You decide to send a message to your friend using the Diffie-Hellman key exchange. You pick p = 78401, g = 26869, and a = 1620. What A must you transmit to your partner? Show all working; if you use any sneaky shortcuts, please explain what you have done. (Shortcuts are useful, not required)
(b) Let’s check the security of our Diffie-Hellman Algorithm. Modify the brute force algorithm form. class (or build your own), and see if you can use it to deduce a, for the A you calculated in the previous question. Hand in your code, along with your calculated value for a.
(c) Get Matlab to print out the first 50 powers of g (that is, print g1, g2, g3...g50). What do you notice? Is this what you expect? Do you believe this will make the Diffie-Hellman key exchange more or less secure than usual? Give two or three sentences explaining your reasoning.
(d) You and your partner decide to select new g and p values. You select p = 98143. After receiving B from your partner, you calculate S = 9815. Use Euclid’s extended algorithm to calculate S−1 mod 98143 by hand. Show all working.
Hint: The algebra here is finicky and it is easy to make a mistake. If you are unsure of your final answer, you can check it by multiplying S × S−1 mod p.
2 Quickfire Questions (8 marks)
What this question is checking?
For each of the question below, I have de代 写Maths 162: Computational Mathematics Assignment 2R
代做程序编程语言scribed the properties of a dice we would like to build.
In each case, either explain why such a dice can not possibly exist, OR determine what numbers we should write on each side of my dice.
(Note: For many of the questions below there may be multiple valid dice. You only need to find one valid dice, or, if the problem is impossible, explain what goes wrong in two or three sentences.)
a) Design a dice with var(X) = 0.
b) Design a dice where every possible value of X is greater that E(X)
c) Design a dice such that P(X = 8|X > 5) = 1/3 and E(X) = 3.
d) Design a dice with P(X < 5) = 1/2 and P(X > 3) = 1/3.
e) Design a dice such that P(X is odd| X is square) = 1/4, and P(X is square| X is odd ) = 1/3. (X is a square numbers if X = k2for some whole number k).
f) Design a dice which has var(X) = 1 = E(X2), and E(X) = 0 = var(X2).
3 A Novel Cipher (8 marks)
For this question we will consider a novel cipher, the pyramid cipher, as described below.
What is this question checking? Your goal in this question it to take the familiar ideas of cryptography and modular arithmetic learned in class, and apply them to a novel circumstance.

a) By hand, use the Pyramid cipher to encrypt the word ‘NILE’.
b) Write a function Pyramid which takes plaintext as input, and gives the Pyramid ciphertext as output. (If you need a reminder of how functions are built in Matlab, flick forward to Q4)
c) Use your code to encrypt the word ‘HIEROGLYPH’.
d) Suppose you are given the ciphertext ‘SZHYRR’. Is it possible to decrypt and find the original text? If it is possible, what was my plaintext? If it is not possible, what goes wrong?
(Hint: It may be best NOT to solve for P1 first. Instead, is there any combination of Ck which will tell you P3? Can you work forward from there?)
e) Suppose you are given the ciphertext ‘COQBP’. Is it possible to decrypt and find the original text? If it is possible, what was my plaintext? If it is not possible, what goes wrong?
(Hint: It may be best NOT to solve for P1 first. Instead it may be easier to find P3 and work from there.)
f) Do you believe the Pyramid cipher is a good cipher? Is it secure? Does it successfully transmit information?
g) Challenge question (zero marks): Which of the following messages is it possible to decrypt: ‘A’, ‘AB’, ‘ABC’, ‘ABCD’, ‘ABCDE’,... ‘ABCDEFGHIJ’ etc.
Based on this, can you determine when the Pyramid cipher is a valid cipher? What is it about our message which makes the Pyramid cypher succeed or fail? Can you explain WHY this occurs?
4 Continuous Random Variables (8 marks)
Suppose I want to create a function which will give me a point (x, y) in the region 0 < y < x2 < 1: Below you will find three possible scripts for implementing this. (You can also find them on the canvas page for the assignment).
What this question is question checking?
Throughout this question we will use the three scripts given to explore how different ways of generating random numbers can lead to different results.

a) Use each of the above functions to create N = 4000 samples. (You don’t need to hand anything in for this question)
b) For each dataset, what is the probability that X < 0.3. (We might call these probabilities P(Xa < 0.3), P(Xb < 0.3), P(Xc < 0.3)).
c) What is the expected value of Y for each data set? (We might call this E(Ya), E(Yb), E(Yc)).
d) For each of the scripts given, give one or two sentences explaining what the script. is doing. In particular, highlight how the three scripts are similar and/or different to one another.
e) Use the scatter command to draw an image representing each of your sample sets. Hand in your three figures, Remember to label your figures ParabowlA,ParabowlB,ParabowlC.
f) Give one or two sentences on what you notice in your three figures. Do your figures match your understanding based on the code?







         
加QQ：99515681  WX：codinghelp
