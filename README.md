# COSC4368-SWI-Prolog
Intro to SWI-Prolog for AI


Consider the following directed graph.

Enter all the edges between two nodes in the graph and the length of the edge as facts using the
connect predicate. (The number next to each edge shows the length of that edge). Some examples
for nodes a and d are as follows:

connect(a,b,5)

connect(a,d,10)

connect(a,c,8)

connect(a,c,8)

connect(d,e,6)

connect(d,f,11)

connect(d,g,4)

Homework 2

COSC4368 Artificial Intelligence Programming
University of Houston
Department of Computer Science
Sent on: February 15, 2017
Due: February 24, 2017

a

b

c

e

d

f

g

5

6

8 10

4

5

1 2

9

2

11

4

Write the necessary Prolog code as rules to answer the following questions (add them to the
knowledge base):

i. Find all the paths between any two nodes in the graph with the total length of the path.

Example:

?- path(a,g,Length,Path).

Length = 11,

Path = abdg ;

Length = 15,

Path = abdeg ;

Length = 19,

Path = abdfg ;

Length = 16,

Path = abeg ;

Length = 14,

Path = adg ;

Length = 18,

Path = adeg ;

Length = 22,

Path = adfg ;

Length = 14,

Path = acfg ;

Length = 16,

Path = acdg ;

Length = 20,

Path = acdeg ;

Length = 24,

Path = acdfg ;

ii. Find the length of any given path.

Example:

?-pathLength([a,b,e,g],Length).

Length = 16 .

*************************************************************

You might need to use the following in-built rule in your code:

atom_concat(Atom1, Atom2, Atom3)

atom_concat forms the concatenation of Atom1 and Atom2 and puts it in Atom3.

Example:

?- A='Second ', 

B='Homework',
 atom_concat(A,B,C).

C = 'Second Homework'.

What you need to deliver:

Each team needs to deliver one source code.

The source code must be in SWI-Prolog. The source code should have enough comments to clarify

what has been done in sections (i) and (ii).

- Please do not send anything other than your source code. It could be in .txt or .pl format.
- Please note that not following the proper instructions will result in loss of marks.
- You can have up to 3 submissions on blackboard but TAs will only grade the last one.
- Read the instructions of the homework carefully. Do not add anything that was not asked in the instructions. If you are not sure about something, ask the TAs by email (allow 24 hours before resending your questions) or attend office hours.
- Start early and send your homework on-time. Submitting homework a few minutes before the deadline is not a good idea. Some students found Blackboard unresponsive in the last minutes before the deadline. To avoid that scenario, send your homework at least a few hours before the deadline. If you have other difficulties regarding Blackboard you should ask the UH Blackboard Support: http://www.uh.edu/blackboard/support/. TAs cannot view a student’s blackboard screen, and cannot help you in that way.
- Late submission penalty is 10 points per day after the deadline. 
