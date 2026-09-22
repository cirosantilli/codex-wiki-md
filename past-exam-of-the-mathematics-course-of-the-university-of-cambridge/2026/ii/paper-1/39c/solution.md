<h1 id="39c/solution">Solution</h1>

↑ **Parent:** [39C](../39c.md)

Boundary-layer theory assumes steady incompressible high-Reynolds-number flow, $\delta/x\ll1$, weak streamwise viscous diffusion, nearly constant [pressure](../../../../../pressure.md) across the layer, and outer [pressure](../../../../../pressure.md) [gradient](../../../../../gradient.md) $-\rho^{-1}p_x=U\,U'$.

For $\phi=-A r^k\cos(k\theta)/k$,

$$
u_r=-Ar^{k-1}\cos k\theta,\qquad u_\theta=Ar^{k-1}\sin k\theta.
$$

At $\theta=\pm\pi/k$ the normal [velocity](../../../../../velocity.md) vanishes; along the upper wall $U(x)=Ax^{k-1}$. [Boundary-layer scaling](../../../../../boundary-layer-scaling.md) gives

$$
\delta=\sqrt{\frac{\nu x}{U}}=(\nu x^{2-k}/A)^{1/2}.
$$

Set $m=k-1$. The [Falkner-Skan equation](../../../../../falkner-skan-equation.md) becomes

$$
f^{(3)}=(k-1)f'^2-\frac{k}{2}ff''+(1-k),
$$

so $\alpha=k-1$, $\beta=-k/2$, $\gamma=1-k$, with  
$f(0)=f'(0)=0$ and $f'(\infty)=1$. Finally

$$
\frac{\delta}{x}=(\nu/A)^{1/2}x^{-k/2}\ll1
$$

requires $x\gg(\nu/A)^{1/k}$; thus $a=1/k$ and the tip region violates the approximation.

## ↑ Ancestors (10)

1. [39C](../39c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
