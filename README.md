Project 0a.

This project is part of Harvard Extension School's 'Introduction to Artifical Intelligence with Python' course, taught by Brian Yu.
https://cs50.harvard.edu/ai/2024/

This was the first of several projects.

**To run**:
python degrees.py {directory-'small' or 'large'-that contains CSVs to run program}

**Goal of program**:
The purpose of Lesson 0 was to learn about various search algorithms, including depth-first search (DFS), breadth-first search (BFS), greedy BFS, etc.

We also learned about Adversarial Search algorithms like minimax and alpha-beta pruning.

In this project, I implemented BFS to solve for the shortest degree of separation between two actors. As an example, Tom Cruise and Demi Moore have starred in the same movie (data provided in CSVs included in this project.) This means that there is only 1 degree of separation between the two actors, as they both starred in 'A Few Good Men.' The program would print out:

1 degrees of separation.
1: Tom Cruise and Demi Moore starred in A Few Good Men

Another example is if 2 actors have starred in different movies, but are connected through a mutual actor who has acted in both films. For example:

2 degrees of separation.
1: Tom Cruise and Kevin Bacon starred in A Few Good Men
2: Kevin Bacon and Bill Paxton starred in Apollo 13

Through building this project, I learned about implementing a queue to solve for getting the shortest path between two people. See the 'shortest_path' function in degrees.py for more.


