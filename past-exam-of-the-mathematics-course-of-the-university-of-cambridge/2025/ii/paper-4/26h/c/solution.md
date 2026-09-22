<h1 id="26h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $h'(x)=-g(x)/x$, the joint density from part (b) can be written

$$
f_{Y,Z}(y,z)=-h'(y+z).
$$

The pieces are therefore independent if and only if

$$
\boxed{-h'(y+z)=h(y)h(z)\quad(y,z\geq0)}.
$$

This condition is also sufficient because $h$ is the common marginal density.

Set $c=h(0)$. Taking $z=0$ gives the differential equation

$$
h'(y)=-c\,h(y).
$$

Since $h$ is a probability density, $c$ must be positive, and normalization gives

$$
\boxed{h(y)=ce^{-cy}\mathbf 1_{\{y\geq0\}}}.
$$

Conversely this function satisfies the displayed factorization. Thus the [exponential characterization by a uniform random split](../../../../../../exponential-characterization-by-a-uniform-random-split.md) shows that

$$
\boxed{Y,Z\text{ are independent }\operatorname{Exp}(c)\text{ variables}}.
$$

Equivalently, $g(x)=-xh'(x)=c^2xe^{-cx}$, so $X$ has the gamma distribution with shape two and rate $c$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26H](../../26h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
