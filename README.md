Project 0a.

This project is part of Harvard Extension School's 'Introduction to Artifical Intelligence with Python' course, taught by Brian Yu.
https://cs50.harvard.edu/ai/2024/

This was the first of several projects.

**To run**
python degrees.py {directory-'small' or 'large'-that contains CSVs to run program}

**Goal of program**
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
----
These were the instructions for this first project:

Specification:
Complete the implementation of the shortest_path function such that it returns the shortest path from the person with id source to the person with the id target.

Assuming there is a path from the source to the target, your function should return a list, where each list item is the next (movie_id, person_id) pair in the path from the source to the target. Each pair should be a tuple of two strings.

For example, if the return value of shortest_path were [(1, 2), (3, 4)], that would mean that the source starred in movie 1 with person 2, person 2 starred in movie 3 with person 4, and person 4 is the target.

If there are multiple paths of minimum length from the source to the target, your function can return any of them.

If there is no possible path between two actors, your function should return None.

You may call the neighbors_for_person function, which accepts a person’s id as input, and returns a set of (movie_id, person_id) pairs for all people who starred in a movie with a given person.

You should not modify anything else in the file other than the shortest_path function, though you may write additional functions and/or import other Python standard library modules.

