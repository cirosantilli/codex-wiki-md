<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $A$ is nonempty, so $0<\alpha\leq1$, and put $a=1_A$. By the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md), $\sum_r|\widehat a(r)|^2=\alpha$. Select the nonzero frequencies

$$
R=\{r\ne0:|\widehat a(r)|\geq\alpha^{3/2}/2\}.
$$

Then $|R|\alpha^3/4\leq\alpha$, giving **$|R|\leq4\alpha^{-2}$**. Outside $R\cup\{0\}$, the fourth Fourier moment has the bound

$$
\sum_{r\notin R\cup\{0\}}|\widehat a(r)|^4
\leq\frac{\alpha^3}{4}\sum_r|\widehat a(r)|^2
=\frac{\alpha^4}{4}.
$$

The fourfold [normalized convolution on a finite group](../../../../../../normalized-convolution-on-a-finite-group.md) $H=a*a*1_{-A}*1_{-A}$ has transform $|\widehat a(r)|^4$, so [Fourier inversion on a finite group](../../../../../../fourier-inversion-on-a-finite-group.md) gives $H(x)=\sum_r|\widehat a(r)|^4e_N(rx)$. It is real and nonnegative, and $H(x)>0$ implies $x\in2A-2A$ because the convolution counts representations, with a positive normalization.

Use the [Bohr set in phase-distance convention](../../../../../../bohr-set-in-phase-distance-convention.md)

$$
B(R,1/10)=\{x:\|rx/N\|_{\mathbb R/\mathbb Z}\leq1/10\text{ for every }r\in R\}.
$$

On this set all retained [additive characters](../../../../../../additive-character.md) have positive real part. The zero-frequency contribution is $\widehat a(0)^4=\alpha^4$, and the total absolute contribution of the discarded frequencies is at most $\alpha^4/4$. Hence

$$
H(x)\geq\alpha^4-\alpha^4/4>0\qquad(x\in B(R,1/10)).
$$

Therefore

$$
\boxed{B(R,1/10)\subseteq A+A-A-A,\qquad |R|\leq4/\alpha^2.}
$$

This is an explicit [Bogolyubov lemma](../../../../../../bogolyubov-lemma.md). In the chord-distance convention for a [Bohr set](../../../../../../bohr-set.md), the phase-radius $1/10$ corresponds to chord radius $2\sin(\pi/10)>1/10$; alternatively the same positivity proof works directly at chord radius $1/10$. Thus the requested lower bound on width holds in either convention. If $R$ is empty, the [Bohr set](../../../../../../bohr-set.md) is the whole group. Nonemptiness of $A$ is necessary for the density statement.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
