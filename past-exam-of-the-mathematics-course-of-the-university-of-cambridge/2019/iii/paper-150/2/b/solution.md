<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose the [sieve distribution](../../../../../../sieve-distribution.md) has the form

$$
|\mathcal A_d|=Xg(d)+r_d\qquad(d\mid P(z)),
$$

where $g$ is a [multiplicative arithmetic function](../../../../../../multiplicative-function.md) on squarefree integers and $0\leq g(p)<1$. Define

$$
h(d)=\prod_{p\mid d}\frac{g(p)}{1-g(p)},\qquad
G(D,z)=\sum_{\substack{\ell<D\\\ell\mid P(z)}}h(\ell).
$$

Then the [Selberg upper-bound sieve](../../../../../../selberg-upper-bound-sieve.md) states

$$
\boxed{
S(\mathcal A,\mathcal P;z)
\leq\frac X{G(D,z)}
+\sum_{\substack{m<D^2\\m\mid P(z)}}3^{\omega(m)}|r_m|
}
$$

for $1<D\leq z$, with immaterial endpoint changes under other level conventions.

To construct the weights, put

$$
G_d(y,z)=
\sum_{\substack{\ell<y\\\ell\mid P(z)\\(\ell,d)=1}}h(\ell)
$$

and set

$$
\lambda_d=
\begin{cases}
\displaystyle
\mu(d)\prod_{p\mid d}(1-g(p))^{-1}
\frac{G_d(D/d,z)}{G(D,z)},&
d<D,\ d\mid P(z),\\[6pt]
0,&\text{otherwise}.
\end{cases}
$$

Then $\lambda_1=1$. If $\gcd(n,P(z))=1$, the divisor sum $\sum_{d\mid n}\lambda_d$ equals one, and hence

$$
1_{\gcd(n,P(z))=1}
\leq\left(\sum_{\substack{d\mid n\\d\mid P(z)}}\lambda_d\right)^2.
$$

Summing against $a_n$ and expanding gives

$$
S(\mathcal A,\mathcal P;z)
\leq\sum_{d,e}\lambda_d\lambda_e
\bigl(Xg([d,e])+r_{[d,e]}\bigr).
$$

The Selberg diagonalization of the positive quadratic form gives

$$
\sum_{d,e}\lambda_d\lambda_e g([d,e])=\frac1{G(D,z)}.
$$

Finally, grouping the error by $m=[d,e]$ gives at most $3^{\omega(m)}$ pairs $(d,e)$ for each squarefree $m$; using $|\lambda_d|\leq1$ yields the stated remainder.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
