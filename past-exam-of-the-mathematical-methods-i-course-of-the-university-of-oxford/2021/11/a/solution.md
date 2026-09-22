<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [integrating factor](../../../../integrating-factor.md) directly solves a linear first-order equation; a general second-order equation needs an additional reduction. There are several sufficient cases, with all divisions restricted to intervals where their denominators are nonzero.

If $A=0$ and $B\ne0$, divide by $B$ to obtain $y'+(C/B)y=D/B$. The integrating factor is $\mu=\exp(\int C/B\,dx)$ and

$$
y=\mu^{-1}\left(K+\int\mu D/B\,dx\right).
$$

If $C=0$ and $A\ne0$, put $u=y'$. Then $u'+(B/A)u=D/A$ is first order, with integrating factor $\nu=\exp(\int B/A\,dx)$; solve for $u$ and integrate once more for $y$.

A further reducible class has $C=B'-A''$, for then

$$
Ay''+By'+Cy=\frac d{dx}\bigl[Ay'+(B-A')y\bigr].
$$

One [integration](../../../../integral-split.md) produces a first-order equation for $y$, whose integrating factor after division by $A$ is $\exp(\int(B-A')/A\,dx)$.

Multiplication can always put a regular second-order equation into self-adjoint form by choosing $w=\exp(\int(B-A')/A\,dx)$, since

$$
w(Ay''+By'+Cy)=(wAy')'+wCy.
$$

However, the remaining $wCy$ term generally prevents one integration from solving it. The [limitations of integrating factors for second-order equations](../../../../limitations-of-integrating-factors-for-second-order-equations.md) explain why this formal transformation alone is not a general solution method. These sufficient classes do not purport to classify every specially solvable coefficient choice.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [11](../../11.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
