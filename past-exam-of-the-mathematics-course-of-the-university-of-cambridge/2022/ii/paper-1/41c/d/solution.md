<h1 id="41c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Since $r^{(k)}=b-Ax^{(k)}=-\nabla f(x^{(k)})$, exact line search minimizes  
$f(x^{(k)}+\alpha r^{(k)})$. Differentiating with respect to $\alpha$ gives

$$
-(r^{(k)})^Tr^{(k)}
+\alpha(r^{(k)})^TAr^{(k)}=0,
$$

so

$$
\boxed{\alpha^{(k)}
=\frac{(r^{(k)})^Tr^{(k)}}
{(r^{(k)})^TAr^{(k)}}}.
$$

Moreover,

$$
r^{(k+1)}=r^{(k)}-\alpha^{(k)}Ar^{(k)},
$$

and substitution of the displayed step size yields

$$
\boxed{(r^{(k)})^Tr^{(k+1)}=0}.
$$

**Thus consecutive residuals are orthogonal.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [41C](../../41c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
