<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $A_0=x(a^*a)$, $B_0=x(b^*b)$ and $c=x(a^*b)$. The preceding reality argument gives $x(b^*a)=\bar c$. Positivity therefore implies, for every $\lambda\in\mathbb C$,

$$
0\leq x((b+\lambda a)^*(b+\lambda a))=B_0+\lambda\bar c+\bar\lambda c+|\lambda|^2A_0.
$$

If $A_0>0$, choose $\lambda=-c/A_0$ to obtain $0\leq B_0-|c|^2/A_0$. If $A_0=0$ and $c\ne0$, choosing $\lambda=-tc$ and letting $t\to\infty$ contradicts positivity. Thus $c=0$ in that case too. This proves the [Cauchy–Schwarz inequality for positive C-star functionals](../../../../../cauchy-schwarz-inequality-for-positive-c-star-functionals.md):

$$
\boxed{|x(a^*b)|^2\leq x(a^*a)x(b^*b).}
$$

Apply it with $a=1_A$, $b=z$. Since $0\leq z^*z\leq\|z\|^21_A$, positivity gives

$$
|x(z)|^2\leq x(1_A)x(z^*z)\leq x(1_A)^2\|z\|^2.
$$

Thus $\|x\|\leq x(1_A)$, while evaluation on $1_A$ gives the reverse inequality. Consequently

$$
\boxed{\|x\|=x(1_A).}
$$

The zero functional is covered as well. In the trivial zero algebra all assertions are immediate, and its state space is empty.

For a nonzero unital [C-star algebra](../../../../../c-star-algebra.md), the set $S_A$ of [state on a C-star algebra](../../../../../state-on-a-c-star-algebra.md) functionals is [convex](../../../../../convex-function.md), since both positivity and evaluation $x(1_A)=1$ are preserved by [convex combinations](../../../../../convex-combination.md). The [norm](../../../../../norm.md) identity places it in the closed dual unit ball. Suppose a state satisfies $x=ty+(1-t)z$, with $0<t<1$ and $\|y\|,\|z\|\leq1$. Evaluating at the unit and taking real parts gives

$$
1=t\operatorname{Re}y(1_A)+(1-t)\operatorname{Re}z(1_A)\leq t+(1-t)=1.
$$

Since both weights are strictly positive, both real parts equal $1$. Also $|y(1_A)|,|z(1_A)|\leq1$, so $y(1_A)=z(1_A)=1$. Hence

$$
1=|y(1_A)|\leq\|y\|\leq1,\qquad1=|z(1_A)|\leq\|z\|\leq1.
$$

The stipulated converse to the [norm](../../../../../norm.md) identity makes $y,z$ positive, so both belong to $S_A$. Therefore **$S_A$ is a [face of a convex set](../../../../../face-of-a-convex-set.md), namely the closed dual unit ball**. More precisely it is the [exposed face of the dual ball defined by the unit](../../../../../exposed-face-of-the-dual-ball-defined-by-the-unit.md), since it is cut out by $\operatorname{Re}x(1_A)=1$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
