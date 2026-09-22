<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [uniform covers theorem](../../../../../uniform-covers-theorem.md) says that if a multiset $\mathcal C$ of coordinate subsets covers every coordinate exactly $k$ times, then a [Euclidean body](../../../../../euclidean-body.md) $S\subseteq\mathbb R^n$ satisfies

$$
|S|^k\leq\prod_{A\in\mathcal C}|S_A|,
$$

where $S_A$ is its [coordinate projection of a Euclidean body](../../../../../coordinate-projection-of-a-euclidean-body.md). Work with bounded Borel bodies, whose projections are [Lebesgue measurable sets](../../../../../lebesgue-measurable-set.md); an empty-coordinate projection has measure one.

Prove the theorem by induction on dimension, with the one-dimensional case immediate. Slice at the last coordinate, writing $S_t\subseteq\mathbb R^{n-1}$. The subsets $A\setminus\{n\}$ still cover each remaining coordinate $k$ times, so induction gives

$$
|S_t|\leq\prod_{A\in\mathcal C}|(S_t)_{A\setminus\{n\}}|^{1/k}.
$$

For $A$ not containing $n$, the projected slice is contained in $S_A$, giving a constant bound. For $A$ containing $n$, its measure is the slice measure $f_A(t)$ of $S_A$. Exactly $k$ members of $\mathcal C$ contain $n$, counted with multiplicity. Integrate and apply [Hölder's inequality](../../../../../holder-s-inequality.md) to those $k$ factors:

$$
|S|\leq\left(\prod_{A\not\ni n}|S_A|\right)^{1/k}
\int\prod_{A\ni n}f_A(t)^{1/k}\,dt
\leq\prod_{A\in\mathcal C}|S_A|^{1/k}.
$$

[Fubini's theorem](../../../../../fubini-s-theorem.md) identifies $\int f_A=|S_A|$, completing the proof. Exact covering is needed for real volumes, which may be smaller than one.

The [Bollobas--Thomason box theorem](../../../../../box-theorem.md) states that there is an [axis-parallel box](../../../../../axis-parallel-box.md) $B$ with $|B|=|S|$ and $|B_A|\leq|S_A|$ for every nonempty coordinate subset $A$. Use the [logarithmic linear program for the box theorem](../../../../../logarithmic-linear-program-for-the-box-theorem.md): if its side lengths are $b_i=e^{x_i}$, maximize $\sum_i x_i$ subject to

$$
\sum_{i\in A}x_i\leq\log|S_A|\qquad(\varnothing\ne A\subseteq[n]).
$$

The [linear program](../../../../../linear-programming.md) is feasible by choosing all $x_i$ sufficiently negative and is bounded above by the full-set constraint. Its dual minimizes $\sum_A\lambda_A\log|S_A|$ subject to $\lambda_A\geq0$ and $\sum_{A\ni i}\lambda_A=1$ for each $i$: precisely a [fractional uniform cover](../../../../../fractional-uniform-cover.md).

The dual feasible polytope is nonempty, bounded and defined by integer coefficients, so an optimal extreme point has rational coordinates. Multiply its weights by a common denominator $k$. The resulting integer [uniform cover](../../../../../uniform-cover.md) and the [uniform covers theorem](../../../../../uniform-covers-theorem.md) give

$$
k\log|S|\leq\sum_A(k\lambda_A)\log|S_A|.
$$

Thus the dual optimum is at least $\log|S|$; weight one on $A=[n]$ attains equality. [Strong duality](../../../../../strong-duality.md) gives a primal optimum $\sum_i x_i=\log|S|$. The corresponding box has the required volume and projected-volume bounds, proving the theorem.

For the [Loomis–Whitney theorem](../../../../../loomis-whitney-inequality.md), take the box supplied by the [Bollobas--Thomason box theorem](../../../../../box-theorem.md). Each side length occurs in exactly $n-1$ projections omitting one coordinate, so

$$
|S|^{n-1}=|B|^{n-1}
=\prod_{i=1}^n|B_{[n]\setminus\{i\}}|
\leq\prod_{i=1}^n|S_{[n]\setminus\{i\}}|.
$$

This is the [Loomis--Whitney inequality](../../../../../loomis-whitney-inequality.md).

For the [three projection areas of a volume-one body](../../../../../three-projection-areas-of-a-volume-one-body.md), necessity is $1=|S|^2\leq abc$. Conversely suppose $abc\geq1$ and set

$$
x=\sqrt{ac/b},\qquad y=\sqrt{ab/c},\qquad z=\sqrt{bc/a}.
$$

The box $[0,x]\times[0,y]\times[0,z]$ has projected areas $a,b,c$ and volume $V=\sqrt{abc}\geq1$. Inside it retain the three slabs

$$
S_t=\{(u,v,w):0\leq u\leq x,\ 0\leq v\leq y,\ 0\leq w\leq z,
\ \min(u/x,v/y,w/z)\leq t\}.
$$

For $t>0$, each projection is the full corresponding rectangle, since the slab in the omitted coordinate supplies every point of that projection. The volume is $V[1-(1-t)^3]$. Choose

$$
t=1-(1-1/V)^{1/3}\in(0,1]
$$

to make the volume one. This is a compact connected union of three positive-thickness boxes. Hence the complete answer is

$$
\boxed{a,b,c>0\quad\text{and}\quad abc\geq1}.
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
