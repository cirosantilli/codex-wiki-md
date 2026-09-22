<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Insert the exact solution and expand about $t=t_{n+2}$. Since $f(y)=y'$ and $f'(y)f(y)=y''$, the left side is

$$
y-hy'+\frac25h^2y''.
$$

The coefficient of $h^jy^{(j)}$ on the right side is

$$
\frac45\frac{(-1)^j}{j!}
+\frac15\frac{(-2)^j}{j!}
+\frac15\frac{(-2)^{j-1}}{(j-1)!}
$$

for $j\geq1$, with the last term absent for $j=0$. These coefficients agree through $j=3$; at $j=4$ the left side minus the right side is $1/10$. Thus the [local truncation error](../../../../../../local-truncation-error.md) is $h^4y^{(4)}/10+O(h^5)$ and the method has order three.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
