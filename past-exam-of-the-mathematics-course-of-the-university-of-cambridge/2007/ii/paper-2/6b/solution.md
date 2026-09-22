<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

First-season recruits in year $n+1$ contribute $\alpha\sigma\gamma X_n$. Seeds produced in year $n-1$ that survive two winters, fail first-season germination and germinate in their second season contribute $\beta\sigma^2(1-\alpha)\gamma X_{n-1}$. Hence

$$
\boxed{X_{n+1}=aX_n+bX_{n-1},\quad a=\alpha\sigma\gamma,\quad b=\beta\sigma^2(1-\alpha)\gamma.}
$$

This treats recruitment from older seeds as absent; otherwise the two-season recurrence would need further terms. The [characteristic polynomial](../../../../../characteristic-polynomial.md) is $r^2-ar-b$. For distinct roots,

$$
\boxed{X_n=A r_+^n+B r_-^n,\qquad r_\pm=\frac{a\pm\sqrt{a^2+4b}}2,}
$$

with constants determined by two initial values. For $b=0,a>0$, the recurrence is first order after the initial step; for $a=b=0$ it gives $X_{n+1}=0$. These describe the zero-root degeneracies without interpreting $0^0$ in the formula.

Since $a,b\ge0$, $|r_-|\le r_+$. The positive root is less than one exactly when $a+b<1$: the [polynomial](../../../../../polynomial-split.md) is nonpositive at zero, has only one positive root, and its value at one is $1-a-b$. Therefore

$$
\boxed{\sigma\gamma[\alpha+(1-\alpha)\beta\sigma]<1\ \Longrightarrow\ X_n\longrightarrow0.}
$$

This is the decay condition for the [two-season seed-bank recurrence](../../../../../two-season-seed-bank-recurrence.md). The deterministic model describes expected or averaged abundance; literal eventual integer extinction requires that interpretation. A corresponding branching model with geometrically decaying expected abundance becomes extinct [almost surely](../../../../../almost-sure-convergence.md), since the [probability](../../../../../probability.md) of any surviving plants is at most the expected number.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
