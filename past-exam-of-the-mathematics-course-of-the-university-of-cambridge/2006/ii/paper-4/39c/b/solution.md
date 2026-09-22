<h1 id="39c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [Fourier mode](../../../../../../fourier-mode.md) $u_m^n=z^ne^{im\theta}$. Put $a=4\mu\sin^2(\theta/2)\ge0$. Its [amplification polynomial of a multistep method](../../../../../../amplification-polynomial-of-a-multistep-method.md) is

$$
\boxed{z^2-(1-3a/2)z-a/2=0}.
$$

The two roots are real, one nonnegative and one nonpositive. For $a>0$, evaluation at $1$ gives $a>0$ and at zero gives $-a/2<0$, so the positive root lies below one. The negative root is at least $-1$ exactly when the value at $-1$, namely $2-2a$, is nonnegative. Thus both roots have modulus at most one exactly for $0\le a\le1$. At $a=0$ they are $1,0$, and at $a=1$ they are $1/2,-1$; all unit-modulus roots are simple, satisfying the multistep [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md). Since the largest available $a$ is $4\mu$, the [Adams-Bashforth stability for centered diffusion](../../../../../../adams-bashforth-stability-for-centered-diffusion.md) condition is

$$
\boxed{0\le\mu\le1/4}.
$$

For $\mu>1/4$, the highest-frequency mode has a root less than $-1$ and grows, proving necessity as well as sufficiency.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39C](../../39c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
