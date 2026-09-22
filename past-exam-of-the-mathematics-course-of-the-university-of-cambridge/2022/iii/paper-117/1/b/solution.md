<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The weighted [sifting function](../../../../../../sifting-function.md) is

$$
S(\mathcal A,\mathcal P,z)
=\sum_{\substack{n\geq1\\(n,P_z)=1}}a_n.
$$

Let $\lambda_1=1$ and let the real [Selberg sieve weights](../../../../../../selberg-upper-bound-sieve.md) $\lambda_d$ vanish unless $d\mid P_z$ and $d\leq D$. Since

$$
1_{(n,P_z)=1}\leq\left(\sum_{d\mid(n,P_z)}\lambda_d\right)^2,
$$

expansion and the distribution hypothesis give

$$
S(\mathcal A,\mathcal P,z)
\leq X\sum_{d,e}\lambda_d\lambda_e g([d,e])
+\sum_{d,e}\lambda_d\lambda_e r_{[d,e]}.
$$

For the optimizing Selberg weights, the main quadratic form is $G(D,z)^{-1}$, where

$$
G(D,z)=\sum_{\substack{\ell\leq D\\\ell\mid P_z}}
\prod_{p\mid\ell}\frac{g(p)}{1-g(p)}.
$$

Thus the general upper bound is

$$
\boxed{
S(\mathcal A,\mathcal P,z)
\leq\frac{X}{G(D,z)}
+\sum_{\substack{d,e\mid P_z\\d,e\leq D}}
|\lambda_d\lambda_e r_{[d,e]}|.}
$$

If the sieve level is instead defined as the largest possible least common multiple, one supports the individual weights on $d\leq\sqrt D$; this is the same statement after replacing $D$ by $\sqrt D$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
