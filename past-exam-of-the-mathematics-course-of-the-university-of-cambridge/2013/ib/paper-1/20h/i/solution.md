<h1 id="20h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First realize the chain as a [random walk on a multigraph](../../../../../../random-walk-on-a-multigraph.md): put three parallel edges between $a,b$, two between $a,c$, and one between $b,c$. There are six edges and vertex degrees $5,4,3$. Choosing an incident edge uniformly gives exactly the stated transition probabilities. The [stationary distribution of a graph random walk](../../../../../../stationary-distribution-of-a-graph-random-walk.md) is the degree divided by twelve, $\pi=(5,4,3)/12$, and detailed balance follows because each edge multiplicity contributes the same flux in both directions.

For the first positive return time, [Kac's lemma](../../../../../../kac-s-lemma.md) gives

$$
\boxed{k(a,a)=1/\pi_a=12/5.}
$$

For passage to $b$, put $h_a=k(a,b)$ and $h_c=k(c,b)$. The first-step equations are $h_a=1+(2/5)h_c$ and $h_c=1+(2/3)h_a$, since reaching $b$ stops the clock. Thus

$$
\boxed{k(a,b)=21/11,\qquad k(c,b)=25/11.}
$$

A multigraph is essential: a simple graph on three vertices cannot have six edges.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
