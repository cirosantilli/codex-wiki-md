<h1 id="39a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [Fourier stability analysis](../../../../../../fourier-stability-analysis.md), substitute $u_j^n=g_n e^{ij\theta}$. The spatial second difference multiplies by $-4\sin^2(\theta/2)$. Set $a=4\mu\sin^2(\theta/2)\geq0$. The mode satisfies

$$
g_{n+1}=(1-\tfrac32a)g_n+\tfrac12a\,g_{n-1},\qquad P(z)=z^2-(1-\tfrac32a)z-\tfrac12a=0.
$$

For $a>0$ the two roots are real of opposite signs. Because $P(0)<0$ and $P(1)=a>0$, the positive root lies strictly between zero and one. The negative root is at least $-1$ exactly when $P(-1)=2-2a\geq0$, namely $a\leq1$. At $a=0$ the roots are $1,0$; at $a=1$ they are $1/2,-1$, all simple. Thus the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) for a stable two-step scheme holds exactly for $0\leq a\leq1$. The discriminant $1-a+(9/4)a^2$ is bounded away from zero on that interval, so the mode powers are uniformly bounded, including the endpoints.

The maximum value of $a$ over all frequencies is $4\mu$, attained at $\theta=\pi$. Therefore

$$
\boxed{\text{the scheme is stable if and only if }0\leq\mu\leq\tfrac14.}
$$

For $\mu>1/4$, the highest-frequency mode has a negative amplification root of modulus greater than one and grows exponentially in the step number.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [39A](../../39a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
