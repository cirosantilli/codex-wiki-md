<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a small $s>0$, for example $s<\sigma/2$, independently of $t$. Taking imaginary parts of the identity in part (a) gives

$$
F(t,a,\sigma)=t^{-\sigma}\int_0^s e^{-Lr}h(r)\,dr
+\operatorname{Im}g(s;t,a,\sigma),\qquad
L=\log t,\quad h(r)=\frac{\sin(ar)}a\Gamma(\sigma+r).
$$

The [parameter-shift remainder bound for a logarithmic Laplace integral](../../../../../../parameter-shift-remainder-bound-for-a-logarithmic-laplace-integral.md) makes the last term $O(t^{-\sigma-s})$, smaller than $t^{-\sigma}L^{-k}$ for every fixed $k$.

The endpoint function $h$ is analytic near zero. For any fixed $N$, its [Taylor expansion](../../../../../../taylor-expansion.md) is

$$
h(r)=\sum_{n=0}^N\frac{h^{(n)}(0)}{n!}r^n+O(r^{N+1}).
$$

Integrating this expansion against $e^{-Lr}$ uses

$$
\int_0^\infty e^{-Lr}r^n\,dr=\frac{n!}{L^{n+1}},
$$

while the error is $O(L^{-N-2})$ and the extension from $s$ to infinity contributes an exponentially small tail. This is [Watson's lemma](../../../../../../watson-s-lemma.md), and gives

$$
\boxed{F(t,a,\sigma)=t^{-\sigma}\left[
\sum_{n=0}^N\frac{\beta_n(a,\sigma)}{(\log t)^{n+1}}
+O\bigl((\log t)^{-N-2}\bigr)\right],\qquad
\beta_n=h^{(n)}(0)}.
$$

Equivalently the coefficients have the stated exponential generating function $h(r)=\sum_{n\ge0}\beta_nr^n/n!$. In particular,

$$
\beta_0=0,\quad\beta_1=\Gamma(\sigma),\quad
\beta_2=2\Gamma'(\sigma),\quad
\beta_3=3\Gamma''(\sigma)-a^2\Gamma(\sigma).
$$

Thus the apparent $t^{-\sigma}(\log t)^{-1}$ term vanishes: the first nonzero terms are $t^{-\sigma}[\Gamma(\sigma)(\log t)^{-2}+2\Gamma'(\sigma)(\log t)^{-3}+\cdots]$. The [derivatives of the gamma function](../../../../../../derivative-of-the-gamma-function.md) supply the successive logarithmic coefficients.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
