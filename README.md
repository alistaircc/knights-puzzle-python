#### **4 Knights Puzzle:**

#### This program which solves the 4 Knight Puzzle Problem for a 3x3 grid was broken down into the following segments:

1.   Successor Function
2.   Heuristic Function
3.   Expand Function
4.   A-Search Function
5.   Branch & Bound Search Function
6.   10 rounds of execution

The data structure used for the solution for both search functions was a queue (Priority Queue). Why? A Priority Queue enabled us to add a cost (i.e. priority) to the element being stored in the queue (making it easy to add the f(n) value for A* and the cost to goal value for Branch & Bound).

> Priority Queue uses Least Cost First Prioritization when getting elements from queue


#### **1. What was used as a measurement system for comparing Search Algorithm effectiveness?**

*   Time taken to find goal state
*   Average of time taken

The reason why in this experiment we basically only measured "Optimality" for the comparative analysis is because we saw from our initial runs we saw that the:
- "Space Complexity" (i.e. the max no. of states in memory) was the same (i.e. all states will be in memory)
-  "Time Complexity" (i.e. the no. of states expanded) was the same (i.e. 16 for both)
- "Completeness" (i.e. the ability for the algorithm to find a solution) was the same (i.e. True for both).

#### **2. What were the results of A* vs Branch & Bound?**

*   A-Search found a solution within 0.005233907699584961 secs on average.
*   Branch & Bound Search found a solution within 0.0070170402526855465 secs on average.

Making **A-Star Search** approx. **0.002 secs** faster at finding an optimal solution.


#### How to Run Program?
1. Clone or download the repo https://github.com/alistaircc/knights-puzzle-python.git
2. Navigate to the directory where repo was downloaded using `cd` cmdline
3. Once in the root of the directory, run `pip install -r requirements.txt` (to install the necessary python lib packages) 
4. Once installation is completed, run program by typing `python 4knights.py`
