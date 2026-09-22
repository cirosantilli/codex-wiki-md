<h1 id="19h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the positive-recurrent case, let $q=p_0+p_1<p$. Detailed balance for the length chain requires

$$
\pi_kq=\pi_{k+1}p,
$$

so, with $r=q/p<1$,

$$
\pi_k=\pi_0r^k.
$$

Normalization gives $\pi_0=1-r$. The self-loop at zero makes the length chain aperiodic, so the convergence theorem for irreducible positive-recurrent aperiodic Markov chains gives

$$
\boxed{
\lim_{n\to\infty}\mathbb P(\ell(X_n)=k\mid X_0=\varnothing)
=\left(1-\frac{p_0+p_1}{p}\right)
\left(\frac{p_0+p_1}{p}\right)^k
}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
