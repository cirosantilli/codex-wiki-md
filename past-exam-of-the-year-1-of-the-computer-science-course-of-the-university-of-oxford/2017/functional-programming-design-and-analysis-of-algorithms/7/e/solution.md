<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The procedure is [Borůvka's algorithm](../../../../../boruvka-s-algorithm.md). In the first round, visiting singleton components in the order $a,b,c,d,e,f,g,h$, the chosen edges are respectively

$$
ac,\ be,\ cf,\ df,\ eh,\ df,\ eg,\ eh.
$$

The set of new edges is **$\{ac,be,cf,df,eh,eg\}$**: repeated selections of $df$ and $eh$ insert no extra copy. The resulting two components are $\{a,c,d,f\}$ and $\{b,e,g,h\}$. Each chooses $fh$ in round two, producing the weight-36 tree from part (d). The within-round order of distinct insertions can therefore be $ac,be,cf,df,eh,eg$, followed by $fh$ in the next round; it need not be the globally sorted Kruskal order.

The required [minimum spanning tree cut property](../../../../../minimum-spanning-tree-cut-property.md) says: for every nonempty proper subset $C\subset V$, the unique minimum-weight edge crossing the cut $(C,V\setminus C)$ belongs to every minimum spanning tree. Indeed, add this edge to a tree that lacks it. The resulting cycle contains another edge crossing the cut, which is strictly heavier; replacing that edge decreases the total weight.

For the general proof, assume all edge weights are distinct. Fix the components at the beginning of a round, as the given procedure does. Each selected edge is the unique lightest edge across one of their cuts, so belongs to every minimum spanning tree. Inductively, the entire selected set is contained in such a tree and is therefore acyclic. While there is more than one component, connectedness supplies an outgoing edge for each, so at least two components merge. The finite process terminates connected. A connected subgraph of a spanning tree must be that whole tree, proving that the returned set is a minimum spanning tree.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
