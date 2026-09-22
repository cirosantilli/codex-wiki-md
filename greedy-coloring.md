# Greedy coloring

↑ **Parent:** [Graph coloring](graph-coloring-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Greedy_coloring)

For a finite [simple graph](simple-graph.md), choose an order of its [vertices](vertex-graph-theory.md) and process them one at a time. Give each [vertex](vertex-graph-theory.md) the smallest positive colour label not already used by its coloured neighbours, and keep all earlier assignments. This is [greedy coloring](greedy-coloring.md): each step makes a locally available choice. The resulting [graph coloring](graph-coloring-split.md) is proper because, for each [edge](edge-of-a-graph.md), its later endpoint avoids the colour of its earlier endpoint.[Leighton, MIT Graph Theory and Coloring, transcript pages 12–13](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/1ccaf180bcd244fddd32e60789fa922f_h9wxtqoa1jY.pdf)

If the [maximum degree of a graph](maximum-degree-of-a-graph.md) is $\Delta(G)$, a [vertex](vertex-graph-theory.md) has at most $\Delta(G)$ previously coloured neighbours, forbidding at most that many distinct colours. At least one label among $1,\ldots,\Delta(G)+1$ remains available. Consequently every order gives

$$
\chi(G)\leq\text{number of colours used by greedy colouring}\leq\Delta(G)+1.
$$

This is an upper bound, not a promise that [greedy coloring](greedy-coloring.md) attains the [chromatic number](chromatic-number.md).[MIT, Graphs and Coloring, Theorem 2](https://ocw.mit.edu/courses/6-1200j-mathematics-for-computer-science-spring-2024/mit6_1200j_s24_lec11.pdf)

<a id="image-two-orders-for-greedy-coloring-of-the-same-path-graph-p-4"></a>
![](greedy-coloring-order.png)

**[Figure 1](#image-two-orders-for-greedy-coloring-of-the-same-path-graph-p-4). Two orders for greedy coloring of the same path graph $P_4$**. The [edges](edge-of-a-graph.md) are $12,23,34$ in both drawings. Each dot shows its assigned colour number, with the [vertex](vertex-graph-theory.md) label above and its processing step below. The order $1,2,3,4$ uses two colours; the order $1,4,2,3$ uses three.

Consider the [path graph](path-graph.md) $P_4$ with [edges](edge-of-a-graph.md) $12,23,34$. In the order $1,2,3,4$, [greedy coloring](greedy-coloring.md) assigns the colours $1,2,1,2$ respectively. In the order $1,4,2,3$, it assigns colours $1,1,2,3$ in processing order: [vertices](vertex-graph-theory.md) $1,4$ both get colour $1$, then [vertex](vertex-graph-theory.md) $2$ gets colour $2$, and finally [vertex](vertex-graph-theory.md) $3$ sees colours $2$ and $1$ at its two neighbours and must take colour $3$. Written in [vertex](vertex-graph-theory.md) order $1,2,3,4$, this second colouring is $1,2,3,1$.

The [path graph](path-graph.md) has [chromatic number](chromatic-number.md) two: the first assignment achieves two colours, and any [edge](edge-of-a-graph.md) rules out one. Its [maximum degree of a graph](maximum-degree-of-a-graph.md) is two, so three colours in the second assignment still satisfy the bound. The extra colour comes entirely from the processing order. The [crown graph](crown-graph.md) gives a larger family where a poor order can make [greedy coloring](greedy-coloring.md) use arbitrarily many colours although the [chromatic number](chromatic-number.md) remains two.

**Table of contents**

- [Extension of a partial colouring by neighbour-colour savings](extension-of-a-partial-colouring-by-neighbour-colour-savings.md)
  - [Neighbour-colour saving](neighbour-colour-saving.md)

## ↑ Ancestors (6)

1. [Graph coloring](graph-coloring-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Chromatic number](chromatic-number.md)
- [Crown graph](crown-graph.md)
- [Greedy coloring](greedy-coloring.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-11/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/17f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/17f/c/solution.md)
