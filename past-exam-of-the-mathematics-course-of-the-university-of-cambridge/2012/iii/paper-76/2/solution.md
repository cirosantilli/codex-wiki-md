<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use primes for differentiation with respect to $X$. Since $X=\epsilon x$, substituting the amplitude-phase representation into the differential equation and separating real and imaginary parts gives

$$
\epsilon^2A''+(k^2-\sigma^2)A=0,\qquad 2\sigma A'+\sigma'A=0.
$$

The second equation is exactly $(\sigma A^2)'=0$. Thus, with a real constant $C$ and $A\ne0$,

$$
\boxed{\sigma A^2=C,\qquad\epsilon^2A''+k^2A=\frac{C^2}{A^3}.}
$$

This [exact amplitude-phase equation](../../../../../exact-amplitude-phase-equation.md) is the [Ermakov-Pinney equation](../../../../../ermakov-pinney-equation.md) for the oscillator. Conversely, any real nonvanishing $A$ satisfying it and $\sigma=C/A^2$ gives an exact complex solution. Existence is not an asymptotic assumption: choose independent real solutions $u,v$ of the original equation, form $y=u+iv$, and set $A=(u^2+v^2)^{1/2}$. Their nonzero constant [Wronskian](../../../../../wronskian.md) prevents simultaneous zeros. The phase derivative satisfies $\sigma A^2=u v_x-u_xv$, so it is constant. Complex conjugation gives a second branch, and linear combinations recover real solutions.

For the [WKB approximation](../../../../../wkb-approximation.md), work on an interval where $K=|k|>0$ is smooth and bounded away from zero. Choose the positive phase branch and an $\epsilon$-independent positive $C$. The equations naturally admit even-power expansions

$$
\sigma=K+\epsilon^2\sigma_1+O(\epsilon^4),\qquad A=A_0+\epsilon^2A_1+O(\epsilon^4).
$$

There is no order-$\epsilon$ phase correction in this convention. Leading order gives $\sigma_0=K$ and $A_0=(C/K)^{1/2}$. Comparing order $\epsilon^2$ in the real equation yields

$$
\sigma_1=\frac{A_0''}{2KA_0}=\frac{3(K')^2}{8K^3}-\frac{K''}{4K^2},\qquad \frac{A_1}{A_0}=-\frac{\sigma_1}{2K}.
$$

Consequently

$$
\boxed{y_0=K^{-1/2}\left[C_+e^{i\epsilon^{-1}\int^XK(s)ds}+C_-e^{-i\epsilon^{-1}\int^XK(s)ds}\right],\qquad\sigma_1=\frac{3(K')^2}{8K^3}-\frac{K''}{4K^2}.}
$$

The constants absorb the normalization. The opposite phase branch changes the sign of $\sigma$ and its correction. A zero of $k$ is a [classical turning point](../../../../../classical-turning-point.md) where this particular expansion fails; the exact amplitude-phase equation itself remains valid for a suitable complex solution.

For the [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md), take $\epsilon=\lambda^{-1/2}$ and use the interval coordinate as $X$, so $K(X)=X+1$ on $[0,1]$. Combining the conjugate branches to satisfy the left Dirichlet [boundary condition](../../../../../boundary-condition.md) produces a sine of the phase integral from zero. The right Dirichlet [boundary condition](../../../../../boundary-condition.md) requires an integer multiple of $\pi$. No turning-point phase shift is present. We have

$$
\int_0^1K\,dX=\frac32,\qquad\int_0^1\sigma_1\,dX=\int_0^1\frac3{8(X+1)^3}\,dX=\frac9{64}.
$$

Thus the [two-term Dirichlet WKB quantization](../../../../../two-term-dirichlet-wkb-quantization.md) is

$$
\frac32\sqrt{\lambda_n}+\frac9{64\sqrt{\lambda_n}}=n\pi+O(\lambda_n^{-3/2}).
$$

Solving first for the square root and then squaring gives

$$
\sqrt{\lambda_n}=\frac{2n\pi}3-\frac9{64n\pi}+O(n^{-3}),\qquad\boxed{\lambda_n=\frac{4\pi^2n^2}{9}-\frac3{16}+O(n^{-2}).}
$$

As an independent sign check, the [Liouville transformation of a second-order equation](../../../../../liouville-transformation-of-a-second-order-equation.md) with $t=X+X^2/2$ and $v=\sqrt{X+1}\,y$ gives $-v_{tt}-3v/[4(2t+1)^2]=\lambda v$ on an interval of length $3/2$. The mean transformed potential is $-3/16$, consistent with the constant spectral correction.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
