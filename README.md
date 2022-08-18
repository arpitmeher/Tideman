# Tideman
PSET3 CS50x-2021 https://cs50.harvard.edu/x/2021/psets/3/tideman/ <br/>
The Tideman voting method (also known as “ranked pairs”) is a ranked-choice voting method that’s guaranteed to produce the Condorcet winner of the election if one exists. <br/>
“Condorcet winner” of the election: the person who would have won any head-to-head matchup against another candidate <br/>
The Tideman method works by constructing a “graph” of candidates, where an arrow (i.e. edge) from candidate A to candidate B indicates that candidate A wins against candidate B in a head-to-head matchup. <br/>

The Tideman method says the winner of the election should be the “source” of the graph (i.e. the candidate that has no arrow pointing at them).

