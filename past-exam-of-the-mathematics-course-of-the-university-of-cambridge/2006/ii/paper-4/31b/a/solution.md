<h1 id="31b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose an analytic square-root branch of $f$ near infinity in a sector. The leading [Liouville–Green approximation](../../../../../../wkb-approximation.md) is

$$
w_\pm(z)\sim f(z)^{-1/4}\exp\left(\pm\int^z\sqrt{f(s)}ds\right),
$$

with successive inverse-power corrections; the two signs give an asymptotic basis in suitable sectors. Since $\sqrt f=\sqrt{f_0}+f_1/(2\sqrt{f_0}z)+\cdots$, the exponent contains a linear term and a logarithm. For the specified $f$, $\sqrt f=1+1/(2z)+7/(8z^2)+\cdots$, explaining $e^zz^{1/2}$ and $e^{-z}z^{-1/2}$ on the positive real axis.

To determine the requested coefficient from the differential equation itself, put $w_1=e^zz^{1/2}h(z)$. Substitution gives

$$
h''+(2+1/z)h'-\frac9{4z^2}h=0.
$$

For $h=1+a_1/z+\cdots$, the order-$z^{-2}$ coefficient is $-2a_1-9/4$. It must vanish, giving

$$
\boxed{a_1=-9/8}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31B](../../31b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
