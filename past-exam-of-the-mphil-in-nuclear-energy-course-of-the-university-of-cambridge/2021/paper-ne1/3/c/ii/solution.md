<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $R_e=R^+$ and apply the stated constant-coefficient [boundary value problem](../../../../../../boundary-value-problem-split.md). A constant particular solution is $-S/(DB^2)$. Regularity at the origin removes $\cos(Br)/r$, so

$$
\phi(r)=A\frac{\sin(Br)}r-\frac{S}{DB^2}.
$$

The outer [boundary condition](../../../../../../boundary-condition.md) gives $A=SR_e/[DB^2\sin(BR_e)]$, hence

$$
\boxed{\phi(r)=\frac{S}{DB^2}\left[\frac{R_e\sin(Br)}{r\sin(BR_e)}-1\right].}
$$

At $r=0$, use the [limit](../../../../../../limit-of-a-function.md) $\sin(Br)/r\to B$ rather than substitute into the apparent $0/0$. The result satisfies both the differential equation and $\phi(R_e)=0$ provided $\sin(BR_e)\ne0$. This is the ideal extrapolated-boundary model specified in the question; a separately resolved outer transport layer would need its own matching conditions.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Module NE1](../../../../paper-ne1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../../split.md)
7. [MPhil in nuclear energy course of the University of Cambridge](../../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
