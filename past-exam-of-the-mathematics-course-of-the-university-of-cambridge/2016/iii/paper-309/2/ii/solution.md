<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $f=1-2M(v)/r$, so $f_r=2M/r^2$ and $f_v=-2M'/r$, where $M'=dM/dv$. Dots in this solution mean derivatives with respect to [proper time](../../../../../../proper-time.md) $\tau$. The [geodesic Lagrangian](../../../../../../geodesic-lagrangian.md) becomes

$$
L=f\dot v^2-2\dot v\dot r-r^2\dot\theta^2-r^2\sin^2\theta\dot\phi^2.
$$

The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) for $r$ gives $\ddot v+(f_r/2)\dot v^2-r(\dot\theta^2+\sin^2\theta\dot\phi^2)=0$. The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) for $v$ gives

$$
2f\ddot v+f_v\dot v^2+2f_r\dot r\dot v-2\ddot r=0.
$$

Eliminate $\ddot v$ between these equations. The two angular [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md) follow by differentiating $-2r^2\dot\theta$ and $-2r^2\sin^2\theta\dot\phi$. Together the four [geodesic equations](../../../../../../geodesic-equation.md) are

$$
\begin{aligned}
0&=\ddot v+\frac{M}{r^2}\dot v^2-r\dot\theta^2-r\sin^2\theta\dot\phi^2,\\
0&=\ddot r+\left(\frac{fM}{r^2}+\frac{M'}r\right)\dot v^2-\frac{2M}{r^2}\dot v\dot r-fr\dot\theta^2-fr\sin^2\theta\dot\phi^2,\\
0&=\ddot\theta+\frac2r\dot r\dot\theta-\sin\theta\cos\theta\dot\phi^2,\\
0&=\ddot\phi+\frac2r\dot r\dot\phi+2\cot\theta\dot\theta\dot\phi.
\end{aligned}
$$

Reading off the symmetric quadratic coefficients gives **all nonzero [Christoffel symbols of the Vaidya metric](../../../../../../christoffel-symbols-of-the-vaidya-metric.md)**:

$$
\boxed{\begin{aligned}
\Gamma^v{}_{vv}&=\frac Mr^2,&
\Gamma^v{}_{\theta\theta}&=-r,&
\Gamma^v{}_{\phi\phi}&=-r\sin^2\theta,\\
\Gamma^r{}_{vv}&=\frac{fM}{r^2}+\frac{M'}r,&
\Gamma^r{}_{vr}&=\Gamma^r{}_{rv}=-\frac Mr^2,&
\Gamma^r{}_{\theta\theta}&=-fr,\\
\Gamma^r{}_{\phi\phi}&=-fr\sin^2\theta,&
\Gamma^\theta{}_{r\theta}&=\Gamma^\theta{}_{\theta r}=\frac1r,&
\Gamma^\theta{}_{\phi\phi}&=-\sin\theta\cos\theta,\\
\Gamma^\phi{}_{r\phi}&=\Gamma^\phi{}_{\phi r}=\frac1r,&
\Gamma^\phi{}_{\theta\phi}&=\Gamma^\phi{}_{\phi\theta}=\cot\theta.
\end{aligned}}
$$

Every unlisted [Christoffel symbol](../../../../../../christoffel-symbol.md) vanishes. The lower-index symmetry is that of the [Levi-Civita connection](../../../../../../levi-civita-connection.md). In particular, the time-dependent mass contributes $+M'/r$ to $\Gamma^r{}_{vv}$; it is absent from $\Gamma^v{}_{vv}$. There are eleven independent nonzero entries, or fifteen when both lower-index orders are counted.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
