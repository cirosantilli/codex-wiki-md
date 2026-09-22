<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

Label the towns $L,M,R$ from left to right, and the treatment plants $A,B,C,D$ as upper-left, upper-right, lower-left and lower-right. Model each [treatment capacity as a sink arc](../../../../../treatment-capacity-as-a-sink-arc.md) to the sea. Incoming untreated sewage can be forwarded, so the numbers inside the plant circles constrain treatment, not total throughput.

The sum of treatment capacities is $16+20+14+12=62$, so no feasible [flow network](../../../../../flow-network.md) can handle more than 62. Here is a feasible routing attaining that upper bound. Send town inflows

$$
L\to A:6,\quad L\to C:9;\qquad M\to A:5,\quad M\to B:7,\quad M\to C:10,\quad M\to D:3;\qquad R\to B:11,\quad R\to D:11.
$$

Every town-to-plant flow respects its directed pipe capacity. Send an additional five units from $C$ to $A$ through their bidirectional pipe, whose capacity is twelve, and two from $D$ to $B$ through their bidirectional pipe, whose capacity is fourteen. Use neither horizontal plant-to-plant pipe.

Now $A$ receives $6+5+5=16$ and treats all of it. Plant $C$ receives $9+10=19$, forwards five and treats fourteen. Plant $B$ receives $7+11+2=20$ and treats all of it. Plant $D$ receives $3+11=14$, forwards two and treats twelve. Thus [flow conservation](../../../../../flow-conservation.md) holds at every plant and all treatment capacities are saturated. The routing proves the upper bound is achievable:

$$
\boxed{\text{maximum total}=62,\qquad (L,M,R)=(15,25,22).}
$$

This is one optimal assignment, not a uniqueness assertion. The total bound comes from the cut consisting of all treatment-to-sea arcs; the explicit routing supplies a matching [maximum flow](../../../../../maximum-flow-problem.md) certificate.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
