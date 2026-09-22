<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Gaussian integers](../../../../../gaussian-integer.md) form an [integral domain](../../../../../integral-domain.md), since they are a [subring](../../../../../subring.md) of the [complex numbers](../../../../../complex-number.md). Use the [Gaussian integer norm](../../../../../gaussian-integer-norm.md)

$$
N(a+bi)=a^2+b^2=|a+bi|^2,
$$

which is a positive [integer](../../../../../integer-split.md) for nonzero $a+bi$ and satisfies $N(\alpha\beta)=N(\alpha)N(\beta)$.

For $\alpha,\beta\in\mathbb Z[i]$ with $\beta\ne0$, write $\alpha/\beta=x+iy$. Choose [integers](../../../../../integer-split.md) $m,n$ with $|x-m|\leq1/2$ and $|y-n|\leq1/2$, put $q=m+in$, and set $r=\alpha-\beta q$. Then

$$
\alpha=\beta q+r,\qquad
N(r)=N(\beta)\big((x-m)^2+(y-n)^2\big)\leq\tfrac12N(\beta)<N(\beta).
$$

Thus division with remainder has either $r=0$ or a strictly smaller [Gaussian integer norm](../../../../../gaussian-integer-norm.md). This proves that $N$ is a [euclidean function](../../../../../euclidean-function.md) and

$$
\boxed{\mathbb Z[i]\text{ is a Euclidean domain}}.
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
