<h1 id="13/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First write the forcing as $\sin x\cos x$. An [integrating factor](../../../../../../integrating-factor.md) for the [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation-split.md) is $e^{-\sin x}$, giving

$$
\frac d{dx}\big(ye^{-\sin x}\big)=\sin x\cos x\,e^{-\sin x}.
$$

Set $u=\sin x$ inside the [antiderivative](../../../../../../antiderivative.md). Then

$$
\int u e^{-u}du=-(u+1)e^{-u}+C,
\qquad y=-(\sin x+1)+Ce^{\sin x}.
$$

The initial value forces $C=1$, hence

$$
\boxed{y(x)=e^{\sin x}-\sin x-1.}
$$

The resulting expression is explicit and valid for all real $x$; the substitution does not impose a global monotonicity condition on $\sin x$ when verifying an [antiderivative](../../../../../../antiderivative.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [13](../../../13.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
