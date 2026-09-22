<h1 id="22h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**No.** In the [Lebesgue space](../../../../../../lp-space.md) $L^1([0,2\pi])$, let

$$
f_n(t)=\sin(nt).
$$

For every $g\in L^\infty([0,2\pi])$, finiteness of the interval gives $g\in L^1([0,2\pi])$, and the [Riemann-Lebesgue lemma](../../../../../../riemann-lebesgue-lemma.md) yields

$$
\int_0^{2\pi}f_n(t)g(t)\,dt\longrightarrow0.
$$

The [duality of Lp spaces](../../../../../../duality-of-lp-spaces.md) therefore shows that $f_n\rightharpoonup0$ in $L^1$. On the other hand,

$$
\lVert f_n\rVert_1
=\int_0^{2\pi}|\sin(nt)|\,dt=4
$$

for every $n$. Thus weak convergence does not imply norm convergence in this $L^1$ space; the [Weakly null sine sequence in L1](../../../../../../weakly-null-sine-sequence-in-l1.md) is the required counterexample.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [22H](../../22h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
