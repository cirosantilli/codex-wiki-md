<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $F=1_A*1_A$. Then $0\leq F\leq1$, $\mathbb EF=\alpha^2$, and the [Parseval identity](../../../../../../parseval-identity.md) gives

$$
\|\widehat F\|_{\ell^1}
=\sum_\gamma|\widehat{1_A}(\gamma)|^2
=\alpha.
$$

Set $d=\lfloor\alpha^2n/(8p^2)\rfloor$. If $d<2$, the asserted integer lower bound is trivial. Otherwise take $q=d$ and $\epsilon=3\alpha/(4p)$ in part b. The resulting subspace $W$ has

$$
\operatorname{codim}W
\leq\frac{4d}{\epsilon^2}
=\frac{64p^2d}{9\alpha^2}
\leq\frac{8n}{9}.
$$

Thus $\dim W\geq n/9>d$, and we may choose a $d$-dimensional subspace $D\leq W$.

For $x\in D$, part b gives

$$
\|\tau_xF-F\|_{L^q}
\leq\epsilon\|\widehat F\|_{\ell^1}
=\frac{3\alpha^2}{4p}.
$$

Apply the supplied maximal inequality to $g(x,y)=F(y+x)-F(y)$. Since $|D|^{1/q}=p$, it gives

$$
\mathbb E_y\sup_{x\in D}|F(y+x)-F(y)|
\leq p\frac{3\alpha^2}{4p}
=\frac{3\alpha^2}{4}
<\mathbb EF.
$$

Hence some $y$ satisfies $F(y)>sup_{x\in D}|F(y+x)-F(y)|$, so $F(y+x)>0$ for every $x\in D$. Since $\operatorname{supp}F=A+A$, this proves

$$
\boxed{y+D\subseteq A+A,
\qquad
\dim D\geq\left\lfloor\frac{\alpha^2n}{8p^2}\right\rfloor.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
