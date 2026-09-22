<h1 id="9d/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Differentiation gives

$$
\frac d{dx}(s(x)^2+c(x)^2)=2sc-2cs=0.
$$

The initial conditions set the constant to one, so

$$
\boxed{s(x)^2+c(x)^2=1},
$$

the [Pythagorean trigonometric identity](../../../../../../../pythagorean-trigonometric-identity.md).

Since $|c|\leq1$, [Taylor theorem with Lagrange remainder](../../../../../../../taylor-theorem-with-lagrange-remainder.md) gives

$$
c(1)=1-\frac12c(\xi)>0
$$

for some $0<\xi<1$, while

$$
c(2)=1-\frac{2^2}{2}+\frac{2^4}{4!}c(\eta)
\leq-1+\frac23<0
$$

for some $0<\eta<2$. The [intermediate value theorem](../../../../../../../intermediate-value-theorem.md) supplies $k\in(1,2)$ with $c(k)=0$. The sine addition formula gives $s(2k)=2s(k)c(k)=0$. The analogous [cosine addition formula](../../../../../../../cosine-addition-formula.md) gives $c(2k)=c(k)^2-s(k)^2=-1$, so

$$
s(x+2k)=-s(x),
\qquad
\boxed{s(x+4k)=s(x)}.
$$

**Thus $s$ is a [periodic function](../../../../../../../periodic-function.md).**

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [9D](../../../9d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
