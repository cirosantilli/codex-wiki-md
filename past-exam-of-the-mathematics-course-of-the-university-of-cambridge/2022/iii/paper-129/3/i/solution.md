<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The finite-field [Bogolyubov lemma](../../../../../../bogolyubov-lemma.md) states that if $A\subseteq G=\mathbb F_p^n$ has density $\alpha$, then $2A-2A$ contains a subspace of codimension at most $2\alpha^{-2}$.

Use normalized [Fourier analysis on a finite abelian group](../../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md) and put $f=1_A$. Define

$$
S=\left\{\gamma\in\widehat G:|\widehat f(\gamma)|\geq\frac{\alpha^{3/2}}{\sqrt2}\right\}.
$$

By [Parseval identity](../../../../../../parseval-identity.md),

$$
|S|\frac{\alpha^3}{2}\leq\sum_\gamma|\widehat f(\gamma)|^2=\alpha,
$$

so $|S|\leq2\alpha^{-2}$. Let

$$
V=\{x\in G:\gamma(x)=1\text{ for every }\gamma\in S\}.
$$

Then $V$ is a subspace of codimension at most $|S|$.

The normalized representation function of $2A-2A$ is

$$
r(x)=(f*f*\widetilde f*\widetilde f)(x)
=\sum_{\gamma\in\widehat G}|\widehat f(\gamma)|^4\gamma(x),
$$

where $\widetilde f(x)=f(-x)$. For $x\in V$, all terms indexed by $S$ are nonnegative real numbers, while

$$
\sum_{\gamma\notin S}|\widehat f(\gamma)|^4
\leq\frac{\alpha^3}{2}\sum_\gamma|\widehat f(\gamma)|^2
=\frac{\alpha^4}{2}.
$$

The trivial character alone contributes $\alpha^4$, so $r(x)>0$. Hence $x\in2A-2A$, proving the [Finite-field Bogolyubov lemma](../../../../../../finite-field-bogolyubov-lemma.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
