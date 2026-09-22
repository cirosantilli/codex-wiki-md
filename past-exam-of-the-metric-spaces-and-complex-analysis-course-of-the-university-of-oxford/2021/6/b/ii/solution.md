<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

The prescribed [pole](../../../../../pole.md) lets us choose $c=4$ and $d=-5-3i$. Write $f(z)=(Az+B)/(4z-5-3i)$. Fixing $1/2$ and $2$ gives

$$
A+2B=-3-3i,\qquad 2A+B=6-6i,
$$

so $A=5-3i$ and $B=-4$. Thus

$$
\boxed{f(z)=\frac{(5-3i)z-4}{4z-5-3i}.}
$$

Its [determinant](../../../../../determinant.md) is $-18\ne0$, so it is a genuine [Möbius transformation](../../../../../mobius-transformation.md). Direct substitution gives $f(1/2)=1/2$, $f(2)=2$, and a pole at $(5+3i)/4$; the numerator at that pole is $9/2\ne0$.

To identify the [image](../../../../../image-of-a-function.md) of the [unit disc](../../../../../unit-disc.md), put

$$
\alpha=\frac4{5-3i}=\frac{10+6i}{17},\qquad
\lambda=-\frac{5-3i}{5+3i}.
$$

Then $|\alpha|^2=8/17<1$, $|\lambda|=1$, and

$$
f(z)=\lambda\frac{z-\alpha}{1-\overline\alpha z}.
$$

In particular, its pole is outside the closed [unit disc](../../../../../unit-disc.md). The identity

$$
1-|f(z)|^2=\frac{(1-|\alpha|^2)(1-|z|^2)}{|1-\overline\alpha z|^2}
$$

shows $f(D)\subseteq D$. For any $|w|<1$, solve $w=\lambda(z-\alpha)/(1-\overline\alpha z)$ to get

$$
z=\frac{w/\lambda+\alpha}{1+\overline\alpha w/\lambda}.
$$

Its denominator is nonzero, and the same [modulus](../../../../../modulus.md) identity for this inverse gives $|z|<1$. Thus $f(D)=D$, and global [injectivity](../../../../../injective-function.md) of a [Möbius transformation](../../../../../mobius-transformation.md) proves the required one-to-one correspondence.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [6](../../../6.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
