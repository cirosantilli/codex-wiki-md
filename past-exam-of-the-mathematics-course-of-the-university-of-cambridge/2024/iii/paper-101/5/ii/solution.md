<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $S=k[x_1,\ldots,x_r]$ with positive degrees $d_i=\deg x_i$, and let $M$ be a finitely generated graded $S$-module whose graded pieces are finite-dimensional over $k$. The [Hilbert-Serre theorem](../../../../../../hilbert-serre-theorem.md) states that

$$
\boxed{H_M(t)=\sum_n\dim_k(M_n)t^n
=\frac{P(t)}{\prod_{i=1}^r(1-t^{d_i})}}
$$

for some Laurent polynomial $P(t)\in\mathbb Z[t,t^{-1}]$. For the standard grading, the [Hilbert function](../../../../../../hilbert-function.md) $n\mapsto\dim_kM_n$ consequently agrees for all sufficiently large $n$ with a polynomial in $n$.

For the proof, induct on $r$. When $r=0$, $M$ is finite-dimensional and its [Hilbert series](../../../../../../hilbert-series.md) is a Laurent polynomial. For $r>0$, multiplication by $x_r$ gives an exact sequence of graded modules

$$
0\longrightarrow K\longrightarrow M(-d_r)
\xrightarrow{x_r}M\longrightarrow C\longrightarrow0.
$$

Both $K$ and $C$ are annihilated by $x_r$, so they are finitely generated graded modules over $k[x_1,\ldots,x_{r-1}]$. Additivity of the Hilbert series yields

$$
(1-t^{d_r})H_M(t)=H_C(t)-H_K(t).
$$

The induction hypothesis supplies the required denominator for the right side and proves the rational formula. When all $d_i=1$, expanding $(1-t)^{-r}$ shows that its coefficients are binomial polynomials in $n$, which proves eventual polynomiality.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
