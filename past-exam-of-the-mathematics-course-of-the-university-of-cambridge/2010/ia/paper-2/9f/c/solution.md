<h1 id="9f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the same first-sex conditioning as in part (b). The conditional [variances](../../../../../../variance-split.md) are $p/q^2$ after a male first capture and $q/p^2$ after a female first capture. Thus

$$
E[\operatorname{Var}(N\mid S)]=\frac{p^2}{q^2}+\frac{q^2}{p^2}.
$$

The conditional [expected values](../../../../../../expected-value.md) are $1+1/q$ and $1+1/p$, with [probabilities](../../../../../../probability.md) $p,q$. A variable taking two values $a,b$ with [probabilities](../../../../../../probability.md) $p,q$ has [variance](../../../../../../variance-split.md) $pq(a-b)^2$, so

$$
\operatorname{Var}(E[N\mid S])=pq\left(\frac1q-\frac1p\right)^2
=\frac{(p-q)^2}{pq}.
$$

The [law of total variance](../../../../../../law-of-total-variance.md) now gives

$$
\boxed{\operatorname{Var}N=\frac{p^2}{q^2}+\frac{q^2}{p^2}
+\frac{(p-q)^2}{pq}
=\frac1{p^2q^2}-\frac3{pq}-2,\qquad q=1-p.}
$$

At $p=q=1/2$ this gives [variance](../../../../../../variance-split.md) $2$, consistent with $N$ being one plus a geometric waiting time of parameter $1/2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
