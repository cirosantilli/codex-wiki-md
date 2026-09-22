<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a based space $(X,x_0)$, the [homotopy group](../../../../../homotopy-group.md)

$$
\pi_k(X,x_0)=[(S^k,*),(X,x_0)]_*
$$

is the set of based homotopy classes, with its usual concatenation operation. A map $f:X\to Y$ is a [weak homotopy equivalence](../../../../../weak-homotopy-equivalence.md) when it induces a bijection on path components and an isomorphism

$$
f_*:\pi_k(X,x)\xrightarrow{\sim}\pi_k(Y,f(x))
$$

for every $k\geq1$ and every basepoint $x$. It is an [n-connected map](../../../../../n-connected-map.md) when it is bijective on $\pi_k$ for $k<n$ and surjective on $\pi_n$; equivalently, every [homotopy fiber](../../../../../homotopy-fiber.md) is $(n-1)$-connected.

A [CW complex](../../../../../cw-complex.md) is built from a discrete set of zero-cells by successively attaching $k$-discs along maps from their boundary spheres, with the weak topology and closure-finiteness conditions. Its filtration by skeleta is the [CW filtration](../../../../../cw-filtration.md).

For any space $X$, form its [singular simplicial set](../../../../../singular-simplicial-set.md) $\operatorname{Sing}X$. Its [geometric realization of a simplicial set](../../../../../geometric-realization-of-a-simplicial-set.md) is a [CW complex](../../../../../cw-complex.md), with one cell for each nondegenerate singular simplex, and evaluation gives

$$
\epsilon:|\operatorname{Sing}X|\longrightarrow X.
$$

The [Simplicial approximation theorem](../../../../../simplicial-approximation-theorem.md) identifies based maps and homotopies from finite simplicial spheres into $|\operatorname{Sing}X|$ with singular simplices in $X$. Consequently $\epsilon$ induces a bijection on components and isomorphisms on all homotopy groups. Thus every space admits a [CW approximation](../../../../../cw-approximation.md).

The vanishing assumptions do not permit removal of all $n$-cells. Take $n=2$ and

$$
X=K(\mathbb Z/r,1),\qquad r>1.
$$

Then $\pi_2(X)=0$, and [homology of a finite cyclic group](../../../../../homology-of-a-finite-cyclic-group.md) gives $H_2(X;\mathbb Z)=0$. If a connected CW complex $Y$ had no two-cells, attaching cells of dimension at least three would not change the fundamental group of its one-skeleton. Hence $\pi_1(Y)$ would be a [free group](../../../../../free-group.md). A weak equivalence $Y\to X$ would instead give $\pi_1(Y)\cong\mathbb Z/r$, which is nontrivial and finite and therefore not free. No such $Y$ exists.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 127](../../paper-127-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
