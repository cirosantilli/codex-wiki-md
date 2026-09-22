<h1 id="14h/solution">Solution</h1>

↑ **Parent:** [14H](../14h.md)

Introduce nonnegative slack variables $s_1,s_3$, a nonnegative surplus variable $s_2$, and an artificial variable $a$. Phase I of the [two-phase simplex method](../../../../../two-phase-simplex.md) minimizes $w=a$. The initial [simplex dictionary](../../../../../simplex-dictionary.md) is

$$
\begin{aligned}
s_1&=9-4x_1-5x_2,\\
a&=12-6x_1-4x_2-x_3+s_2,\\
s_3&=3-3x_1-2x_2+x_3,\\
w&=12-6x_1-4x_2-x_3+s_2.
\end{aligned}
$$

With the nonbasic variables zero this is feasible for the artificial problem. Enter $x_1$; the minimum ratios are $9/4,12/6,3/3$, so $s_3$ leaves. Solving its row for $x_1$ and substituting gives

$$
\begin{aligned}
x_1&=1-\frac23x_2+\frac13x_3-\frac13s_3,\\
s_1&=5-\frac73x_2-\frac43x_3+\frac43s_3,\\
a&=6-3x_3+s_2+2s_3,\\
w&=6-3x_3+s_2+2s_3.
\end{aligned}
$$

Now enter $x_3$. The ratios from decreasing basic variables are $5/(4/3)=15/4$ and $6/3=2$, so $a$ leaves. The resulting dictionary is

$$
\begin{aligned}
x_3&=2+\frac13s_2+\frac23s_3-\frac13a,\\
x_1&=\frac53-\frac23x_2+\frac19s_2-\frac19s_3-\frac19a,\\
s_1&=\frac73-\frac73x_2-\frac49s_2+\frac49s_3+\frac49a,\\
w&=a.
\end{aligned}
$$

Setting the nonbasic variables zero gives $a=0$, so Phase I has reached its minimum and found feasibility. Remove $a$ and reinstate the true objective $z$. Substitution of the basic variables gives

$$
z=\frac{103}{3}-\frac{46}{3}x_2+\frac{44}{9}s_2+\frac{73}{9}s_3.
$$

Enter $x_2$. The decreasing rows give ratios $(5/3)/(2/3)=5/2$ for $x_1$ and $(7/3)/(7/3)=1$ for $s_1$, so $s_1$ leaves. Phase II then has

$$
\begin{aligned}
x_2&=1-\frac37s_1-\frac4{21}s_2+\frac4{21}s_3,\\
x_1&=1+\frac27s_1+\frac5{21}s_2-\frac5{21}s_3,\\
x_3&=2+\frac13s_2+\frac23s_3,\\
z&=19+\frac{46}{7}s_1+\frac{164}{21}s_2+\frac{109}{21}s_3.
\end{aligned}
$$

Every nonbasic variable is nonnegative and every [reduced cost](../../../../../reduced-cost.md) is positive. Thus the [simplex optimality criterion](../../../../../simplex-optimality-criterion.md) proves

$$
\boxed{(x_1,x_2,x_3)=(1,1,2),\qquad z_{\min}=19}.
$$

All three original constraints are active. Positivity of all three [reduced costs](../../../../../reduced-cost.md) also proves uniqueness: equality in the objective lower bound forces $s_1=s_2=s_3=0$, which fixes the displayed solution.

## ↑ Ancestors (10)

1. [14H](../14h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
