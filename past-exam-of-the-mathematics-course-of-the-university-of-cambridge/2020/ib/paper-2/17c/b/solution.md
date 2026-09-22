<h1 id="17c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand the exact solution about $t_{n+1}=t$. The left side is

$$
y(t+h)-y(t)
=hy'+\frac{h^2}{2}y''
+\frac{h^3}{6}y'''
+\frac{h^4}{24}y^{(4)}+O(h^5).
$$

Since $f(t,y(t))=y'(t)$, the right side expands as

$$
hy'
+h^2(1+2\alpha+\beta)y''
+\frac{h^3}{2}(1-\beta)y'''
+\frac{h^4}{6}(1+2\alpha+\beta)y^{(4)}
+O(h^5).
$$

The $hy'$ terms agree for every $\alpha,\beta$, so the method is always consistent and is generically of order one.

The method is explicit exactly when $1+\alpha=0$. With $\alpha=-1$, its $h^2$ defect vanishes only for $\beta=3/2$, so a generic explicit member has order one; that exceptional explicit member has order two and cannot satisfy the next order condition.

For the unrestricted method to have order at least three, the $h^2$ and $h^3$ coefficients must agree:

$$
1+2\alpha+\beta=\frac12,
\qquad
\frac{1-\beta}{2}=\frac16.
$$

Solving gives

$$
\boxed{\alpha=-\frac7{12},
\qquad
\beta=\frac23}.
$$

For these values, $1+2\alpha+\beta=1/2$, so the right-side $h^4$ coefficient is $1/12$, different from the left-side coefficient $1/24$. Hence the order is exactly three.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17C](../../17c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
