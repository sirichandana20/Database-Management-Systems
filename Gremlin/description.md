Graph DB using Tinkerpop and Gremlin


Consider the following graph that lists courses (circles) and prereq relationships (black arrows). Eg. CS101 is a prereq for CS201, and CS334, for CS400 (and so on). The two orange arrows are 'coreqs' (courses that may be taken together, possibly upon instructor approval for example). The orange arrows obviously lead to double connections: between CS420 and CS220, and between CS526 and CS400. If you'd like to think of nodes in terms of nouns, and edges in terms of verbs, our two kinds of edges would be 'requires pre-req' and 'is a co-req of'. 



Q1. Write a Gremlin command that creates the above graph [hint - you will also need a 'traversal' for it]. The command could be a multi-statement one, or a single line one (with function chaining). 

Q2. Write a query that will output JUST the doubly-connected nodes. 

Q3. Write a query that will output all the ancestors (for us, these would be prereqs) of a given vertex. 

Q4. Write a query that will output the max depth starting from a given node (provides a count (including itself) of all the connected nodes till the deepest leaf). This would give us a total count of the longest sequence of courses that can be taken, after having completed a prereq course.

Q5.(a) Write a command that creates a graph of the 7 bridges and 4 regions of Konigsberg. 

(b) Write an 'Eulerian circuit' detection query that runs on your graph, that outputs 'false' (to signify what Euler showed - that there is NO path through the bridges and cities where, starting at any region of the city you traverse each bridge just once, and return to the starting point, ie. there is no closed path, aka circuit). If the graph were modified (eg. an existing bridge is removed, and a new one is added) so there is now an Eulerian circuit, your query needs to emit 'true' for such a case. Note - there is no need to output the sequence of nodes in the circuit (when there is a circuit), just outputting 'true' will do; in other words, your query just needs to report on the presence/absence of a circuit, which is much easier to do than to make it compute an Eulerian closed path if one does exist.
