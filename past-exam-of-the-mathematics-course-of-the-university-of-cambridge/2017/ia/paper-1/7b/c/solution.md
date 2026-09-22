<h1 id="7b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In odd dimension,

$$
\det A=\det A^T=\det(-A)=-\det A,
$$

so $\det A=0$. Since $A$ is real, its [kernel](../../../../../../kernel-of-a-linear-map.md) contains a nonzero real vector $a$.

The plane $a^\perp$ is invariant under $A$, because $a\mathbin{\cdot}Ab=-(Aa)\mathbin{\cdot}b=0$. On this two-dimensional plane, $Ab$ is perpendicular to $b$. Put $|Ab|=\theta|b|$ with $\theta>0$. Then $A^2b$ is parallel to $b$, and

$$
b\mathbin{\cdot}A^2b=-(Ab)\mathbin{\cdot}(Ab)=-\theta^2|b|^2,
$$

so

$$
\boxed{A^2b=-\theta^2b}.
$$

The [matrix exponential](../../../../../../matrix-exponential.md) fixes the kernel vector:

$$
\boxed{e^Aa=a}.
$$

Separating even and odd powers in its series and using $A^{2j}b=(-1)^j\theta^{2j}b$ gives

$$
\boxed{e^Ab=\cos\theta\,b+\frac{\sin\theta}{\theta}Ab}.
$$

Thus $e^A$ acts as a rotation through angle $\theta$ on $a^\perp$ and fixes its axis $\mathbb Ra$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
