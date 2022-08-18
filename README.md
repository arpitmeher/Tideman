# Tideman
PSET3 CS50x-2021 https://cs50.harvard.edu/x/2021/psets/3/tideman/ <br/>
The Tideman voting method (also known as “ranked pairs”) is a ranked-choice voting method that’s guaranteed to produce the Condorcet winner of the election if one exists. <br/>
“Condorcet winner” of the election: the person who would have won any head-to-head matchup against another candidate <br/>
The Tideman method works by constructing a “graph” of candidates, where an arrow (i.e. edge) from candidate A to candidate B indicates that candidate A wins against candidate B in a head-to-head matchup. <br/>

The Tideman method says the winner of the election should be the “source” of the graph (i.e. the candidate that has no arrow pointing at them). <br/>

The preference of the all the voters are recorded. Then all pairs of candidate in which one is preferred over the other are added to an array and then sorted in the decreasing order of the strength of the victory. After the sorting the pairs are locked by adding edges to the graph in decreasing order such that no cycle is formed. When we are done with the locking the 'Source' of thr graph will give us the winner of election. 

