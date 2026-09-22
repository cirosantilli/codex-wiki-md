<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $g(x)=\mu-x^2$ and $f_L(x)=-\operatorname{sgn}(x)g(x)$. Suppose first that $g^k(x)\ne0$ for $0\le k<n$, so no critical hit occurs before the final iterate. Set $A_n=(-1)^n\prod_{k=0}^{n-1}\operatorname{sgn}(g^k(x))\in\{1,-1\}$. The case $n=1$ is the defining identity. If $f_L^n(x)=A_ng^n(x)$ and $g^n(x)\ne0$, evenness of $g$ and oddness of $f_L$ away from zero give

$$
f_L^{n+1}(x)=f_L(A_ng^n(x))
=-A_n\operatorname{sgn}(g^n(x))g^{n+1}(x)=A_{n+1}g^{n+1}(x).
$$

Induction proves the [sign lift of an even map](../../../../../../sign-lift-of-an-even-map.md) formula

$$
\boxed{f_L^n(x)=(-1)^n g^n(x)\prod_{k=0}^{n-1}\operatorname{sgn}(g^k(x))}
$$

on noncritical orbit segments. A final zero value is harmless; using oddness at zero in a subsequent step is not.

The PDF's assertion that this holds for every $x$ is false with its stated $\operatorname{sgn}(0)=1$ convention. For $\mu>0$, choose $x=\sqrt\mu$. Then $g(x)=f_L(x)=0$, so

$$
f_L^2(x)=f_L(0)=-\mu,
$$

but the proposed right side for $n=2$ is $g^2(x)\operatorname{sgn}(x)\operatorname{sgn}(g(x))=+\mu$. This explicit counterexample identifies the missing noncritical qualification. An exact recurrence valid even at critical hits can instead be written with $y_k=g^k(x)$ and $f_L^k(x)=A_ky_k$: start with $A_0=1$, and update

$$
A_{k+1}=\begin{cases}-A_k\operatorname{sgn}(y_k),&y_k\ne0,\\-1,&y_k=0.\end{cases}
$$

The second rule resets the sign because $f_L(0)=-g(0)$ independently of the previous sign. This proves the intended identity wherever it is valid and accounts for the exceptional critical itineraries without changing the map's definition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
