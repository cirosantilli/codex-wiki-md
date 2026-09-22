<h1 id="15g/solution">Solution</h1>

↑ **Parent:** [15G](../15g.md)

For $y=e^{-x}$, substitution in the unnormalized equation gives $[(x+2)-(x+1)-1]e^{-x}=0$. For $y=ax+b$, the remaining expression is $(x+1)a-(ax+b)=a-b$. Thus an independent second solution is $x+1$. Their [Wronskian](../../../../../wronskian.md) is $-(x+2)e^{-x}$, nonzero on $x\geq0$.

The left boundary solution is $u(x)=x+1$, since $u'(0)=u(0)=1$; the decaying right solution is $v(x)=e^{-x}$. A [Robin half-line Green function from left and right solutions](../../../../../robin-half-line-green-function-from-left-and-right-solutions.md) must be continuous at $x=\xi$, while its derivative jumps by one because the leading coefficient of $L$ is one. These conditions give

$$
G(x,\xi)=\frac{u(\min(x,\xi))v(\max(x,\xi))}{W(\xi)},\qquad W(\xi)=-(\xi+2)e^{-\xi}.
$$

Therefore

$$
\boxed{G(x,\xi)=\begin{cases}-\dfrac{x+1}{\xi+2},&0\leq x<\xi,\\-\dfrac{\xi+1}{\xi+2}e^{\xi-x},&x>\xi.\end{cases}}
$$

The two values agree at $x=\xi$, and $G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=(\xi+1)/ (\xi+2)+1/(\xi+2)=1$. Each branch solves the homogeneous equation and its relevant boundary condition, so these checks prove the distributional identity $LG=\delta$ rather than merely postulate the kernel.

Integrate this [Green function](../../../../../green-s-function.md) against the forcing $-(\xi+2)e^{-\xi}$. Splitting at $\xi=x$ gives

$$
y(x)=e^{-x}\int_0^x(\xi+1)d\xi+(x+1)\int_x^\infty e^{-\xi}d\xi=\boxed{\left(\frac{x^2}{2}+2x+1\right)e^{-x}.}
$$

It has $y(0)=y'(0)=1$ and decays at infinity. Direct substitution gives $L[y]=-(x+2)e^{-x}$. Uniqueness follows because a decaying homogeneous solution must be a multiple of $e^{-x}$, and its left boundary condition would require $-c=c$, forcing $c=0$.

## ↑ Ancestors (10)

1. [15G](../15g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
