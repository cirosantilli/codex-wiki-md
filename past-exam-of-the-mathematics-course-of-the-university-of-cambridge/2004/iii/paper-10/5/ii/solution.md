<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The inequality printed in this part is false for general positive functionals.** In $A=M_2(\mathbb C)$ take the [state on a C-star algebra](../../../../../../state-on-a-c-star-algebra.md) $f(a)=a_{22}$ and $x=y=E_{12}$. It is positive since $f(z^*z)=\|ze_2\|^2\geq0$, and it has norm one. But

$$
x^*y=E_{22},\qquad xx^*=yy^*=E_{11},\qquad |f(x^*y)|^2=1,\quad f(xx^*)f(yy^*)=0.
$$

Thus the literal requested inequality would say $1\leq0$.

The correct [Cauchy–Schwarz inequality for positive C-star functionals](../../../../../../cauchy-schwarz-inequality-for-positive-c-star-functionals.md) keeps the orders consistent:

$$
\boxed{|f(x^*y)|^2\leq f(x^*x)f(y^*y).}
$$

To prove it, set $a=f(x^*x)$, $d=f(y^*y)$ and $b=f(x^*y)$. By part (i) and positivity,

$$
0\leq f((x+ty)^*(x+ty))=a+2\operatorname{Re}(tb)+|t|^2d\qquad(t\in\mathbb C).
$$

If $d>0$, choose $t=-\overline b/d$ to obtain $|b|^2\leq ad$. If $d=0$, arbitrary choices of $t$ force $b=0$, and the inequality again follows. Replacing $x,y$ by $x^*,y^*$ also yields the valid alternative

$$
\boxed{|f(xy^*)|^2\leq f(xx^*)f(yy^*).}
$$

Either replacing the printed right-hand factors by $f(x^*x),f(y^*y)$, or replacing the left-hand product by $xy^*$, repairs the statement. No tracial hypothesis is supplied, so it cannot be silently used to exchange those products.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
