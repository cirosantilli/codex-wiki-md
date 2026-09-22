<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For large $t$, write the [survival function](../../../../../../survival-function.md) as

$$
\overline F(t)=t^{-2}\ell(t),\qquad \ell(t)=\frac{C}{\log t\,\log\log t}.
$$

A positive [function](../../../../../../function-split.md) $\ell$ is [slowly varying](../../../../../../slowly-varying-function.md) if $\ell(tu)/\ell(t)\to1$ for every fixed $u>0$. Here

$$
\frac{\ell(tu)}{\ell(t)}
=\frac{\log t\,\log\log t}{\log(tu)\,\log\log(tu)}\longrightarrow1,
$$

since $\log(tu)=\log t+\log u$ and $\log\log(tu)-\log\log t\to0$. Thus $\overline F$ has [regular variation](../../../../../../regular-variation.md) of index $-2$.

The relevant extreme-value criterion is that an infinite right endpoint and a [survival function](../../../../../../survival-function.md) regularly varying with index $-r$, $r>0$, give attraction to the standard [Fréchet distribution](../../../../../../frechet-distribution.md) of shape $r$. Its [distribution function](../../../../../../cumulative-distribution-function.md) is $G_r(x)=e^{-x^{-r}}$ for $x>0$ and zero for $x\leq0$. Here is a direct verification, so no additional theorem is needed to establish the criterion in this example. Choose $a_n\to\infty$ satisfying $n\overline F(a_n)\to1$ and set $b_n=0$. For $x>0$,

$$
n\overline F(a_nx)
=n\overline F(a_n)\frac{\overline F(a_nx)}{\overline F(a_n)}\longrightarrow x^{-2}.
$$

If $u_n\to0$ and $nu_n\to c$, then $n\log(1-u_n)=-nu_n+O(nu_n^2)\to-c$. Applying this with $u_n=\overline F(a_nx)$ gives $F(a_nx)^n\to e^{-x^{-2}}$. For $x\leq0$, the [distribution function](../../../../../../cumulative-distribution-function.md) is zero because the observations are supported on $[10,\infty)$. Therefore

$$
\boxed{G(x)=\begin{cases}e^{-x^{-2}},&x>0,\\0,&x\leq0,\end{cases}\qquad F\in D(G).}
$$

For example, elementary asymptotic normalizers are

$$
a_n=\left(\frac{2Cn}{\log n\,\log\log n}\right)^{1/2},\qquad b_n=0,
$$

for sufficiently large $n$, with arbitrary positive definitions at smaller indices. Indeed $\log a_n\sim\tfrac12\log n$ and $\log\log a_n\sim\log\log n$, so $a_n^2\log a_n\log\log a_n\sim Cn$. The precise valid choice of $C$ at the lower endpoint does not change the limiting shape.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
