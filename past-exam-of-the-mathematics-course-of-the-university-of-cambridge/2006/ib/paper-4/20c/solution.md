<h1 id="20c/solution">Solution</h1>

↑ **Parent:** [20C](../20c.md)

Use [two-phase simplex](../../../../../two-phase-simplex.md) to handle the constraint of the opposite inequality direction. Introduce nonnegative slack variables $s_1,s_2$, a surplus variable $s_3$, and an artificial variable $a$. The equality constraints are

$$
x_1+x_2+x_3+s_1=30,\qquad2x_1-x_2+s_2=35,\qquad
x_1+2x_2-x_3-s_3+a=40.
$$

For Phase I maximize $w=-a$, initially with basis $(s_1,s_2,a)$. Its initial [simplex dictionary](../../../../../simplex-dictionary.md) is

$$
s_1=30-x_1-x_2-x_3,\quad s_2=35-2x_1+x_2,\quad a=40-x_1-2x_2+x_3+s_3,
$$



$$
w=-40+x_1+2x_2-x_3-s_3.
$$

Choose $x_1$ to enter. The [simplex ratio test](../../../../../simplex-ratio-test.md) compares $30$, $35/2$ and $40$, so $s_2$ leaves. The new dictionary is

$$
x_1=\frac{35}{2}+\frac{x_2}{2}-\frac{s_2}{2},\quad
s_1=\frac{25}{2}-\frac32x_2-x_3+\frac12s_2,\quad
a=\frac{45}{2}-\frac52x_2+x_3+\frac12s_2+s_3.
$$

Since $w=-45/2+(5/2)x_2-x_3-s_2/2-s_3$, choose $x_2$ to enter. Its limiting ratios are $25/3$ from $s_1$ and $9$ from $a$, so $s_1$ leaves. This gives

$$
x_2=\frac{25}{3}-\frac23x_3+\frac13s_2-\frac23s_1,
$$



$$
x_1=\frac{65}{3}-\frac13x_3-\frac13s_2-\frac13s_1,\qquad
a=\frac53+\frac83x_3-\frac13s_2+\frac53s_1+s_3.
$$

Now $w=-5/3-(8/3)x_3+s_2/3-(5/3)s_1-s_3$, so let $s_2$ enter. Its limiting ratios are $65$ from $x_1$ and $5$ from $a$; the artificial variable leaves. The [simplex dictionary](../../../../../simplex-dictionary.md) becomes

$$
s_2=5+8x_3+5s_1+3s_3-3a,
$$



$$
x_1=20-3x_3-2s_1-s_3+a,\qquad x_2=10+2x_3+s_1+s_3-a.
$$

Setting all nonbasic variables to zero gives $a=0$, a feasible original basis. Since $-a\leq0$, Phase I is optimal with value zero; delete $a$.

For Phase II the original objective in this basis is

$$
z=50x_1-30x_2+x_3=700-209x_3-130s_1-80s_3.
$$

All nonbasic reduced costs are strictly negative, so no further improving simplex pivot exists. As the nonbasic variables are nonnegative, the dictionary also directly certifies $z\leq700$, with equality only when $x_3=s_1=s_3=0$. Therefore

$$
\boxed{(x_1,x_2,x_3)=(20,10,0),\qquad z_{\max}=700.}
$$

The second original constraint has slack five and the other two are tight. As an independent [linear programming optimality certificate](../../../../../linear-programming-optimality-certificate.md), multiply the first constraint by $130$ and the third, after reversing it, by $80$. This gives $50x_1-30x_2+210x_3\leq700$, and subtracting $209x_3\geq0$ proves the same upper bound for the objective.

## ↑ Ancestors (10)

1. [20C](../20c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
