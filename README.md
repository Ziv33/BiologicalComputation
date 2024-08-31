# Biological Computation - Final Project
## Authors
* Ziv Chaba
* Bar Zomer

Questions can be directed to zivchaba1000@gmail.com
## Assignment
In the first part of the project, we wrote a python code that finds all the monotonic regulation conditions of the reasoning engine that satisfy monotonic requirement and consider whether none, some or all of the activators / inhibitors are present, as we studied in class.

We found 18 monotonic regulation conditions, as expected in the assignment file, and compared it with given table of the assignment.

Our results were a perfect (reordered) equivilant of the 18 conditions of table 2.

## Files
### BasicSystem.py
A file for class BasicSystem(n,m,target). represents an instance in the basic system, contains activators count (int), inhibitors count (int), and the system target (boolean for result - active or inactive).

IN, AC are static variables that represent the maximum count of activators/inhibitors in the system (as per assignment requirements it was set to 2).

The function generateAllNecessaryBasicMonotonicRegulationConditions() is used to generate the basic regulation conditions which correspond to the necessary conditions of monotonic regulation conditions for each of the basic systems.
### main.py
A main file for the project.

The function generateAllBasicSystems(IN,AC) generates every BasicSystem object within the range of activators and inhibitors in this assignment (0-2). Each basic system corresponds to a basic monotonic condition (minimum activators, minimum inhibitors).

After that, with those basic monotonic regulation conditions we expand and complete our set of monotonic regulation conditions by 
committing monotonicity-preserving operations for boolean functions - AND , OR, between the basic monotonic regulation conditions (functions) that we have already found.

Finally, the code outputs a list of all monotonic functions it has calculated for the system, and for each instance - whether it will activate or not (target=True/False).

## Results
The output of the program is as follows:

![Part 1 Program Printout](https://github.com/user-attachments/assets/3893bf86-25c6-4f68-97d7-d396d4feb366)

we have organzied our output, ordered it in accordance with given table's ordering, and visualized it:

![image (5)](https://github.com/user-attachments/assets/48f79311-2d9e-403c-a97f-0bcdb3db7294)

And as you can see, it corresponds with the expected results in the given table:

![image (6)](https://github.com/user-attachments/assets/4dc36535-2def-4b1e-917d-153b231b3bb5)



## How To Run The Program
* Download BasicSystem.py , main.py to your local computer.
* Open command line at their location
* run the command   *python main.py*

Alternatively, you can run this python project on every python IDE.
