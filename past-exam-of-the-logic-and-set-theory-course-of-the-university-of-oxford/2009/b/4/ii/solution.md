<h1 id="b/4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For fixed $\beta$, the recursion defining $\beta+\alpha$ makes it continuous in $\alpha$ at every nonzero limit, and $(\beta+\alpha)+1>\beta+\alpha$. Thus **$\alpha\mapsto\beta+\alpha$ is normal**, including when $\beta=0$.

For $\beta>0$, take $\lambda=\beta\cdot\omega$. If $\alpha<\lambda$, choose a [natural number](../../../../../natural-number.md) $n$ with $\alpha<\beta n$; then $\alpha+\beta\leq\beta(n+1)<\lambda$. Since $\alpha+\beta\geq\alpha$, their [supremum](../../../../../supremum.md) as $\alpha\uparrow\lambda$ is $\lambda$. But $\lambda+\beta>\lambda$, so

$$
\sup_{\alpha<\lambda}(\alpha+\beta)=\lambda<\lambda+\beta.
$$

Hence right addition by a nonzero fixed [ordinal](../../../../../ordinal-split.md) fails continuity and is not normal.

[Normality and argument order in ordinal arithmetic](../../../../../normality-and-argument-order-in-ordinal-arithmetic.md) also give the multiplication statements: **$\alpha\mapsto\beta\cdot\alpha$ is normal for $\beta>0$, while $\alpha\mapsto\alpha\cdot\beta$ is normal exactly when $\beta=1$**. At $\beta=0$ it is constant. For fixed $\beta>1$, let $\kappa=\omega^{\beta\cdot\omega}$. [Cantor normal form](../../../../../cantor-normal-form.md) shows that $\xi\beta<\kappa$ whenever $\xi<\kappa$: leading exponents below $\beta\omega$ remain below it after adding the leading exponent of $\beta$. Thus $\sup_{\xi<\kappa}\xi\beta=\kappa$, but $\kappa\beta>\kappa$, again violating continuity. Left-fixed multiplication is strictly increasing and continuous by its recursion.

For exponentiation, **$\alpha\mapsto\beta^\alpha$ is normal for $\beta\geq2$; bases zero and one are exceptions. The reverse map $\alpha\mapsto\alpha^\beta$ is normal exactly when $\beta=1$**. Exponent zero gives the constant one. For $\beta>1$, use the same $\kappa$ and put $\lambda=\omega^\kappa$. For each $\alpha<\lambda$ choose $0<\zeta<\kappa$ with $\alpha\leq\omega^\zeta$. Then $\alpha^\beta\leq\omega^{\zeta\beta}<\lambda$, while $\alpha^\beta\geq\alpha$ for positive $\alpha$. Consequently its left [supremum](../../../../../supremum.md) is $\lambda$, but $\lambda^\beta=\omega^{\kappa\beta}>\lambda$. The bound by $\omega^\zeta$ also handles finite bases, where an unqualified leading-exponent multiplication formula would need care. All these are [ordinal](../../../../../ordinal-split.md) facts and use no choice.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
