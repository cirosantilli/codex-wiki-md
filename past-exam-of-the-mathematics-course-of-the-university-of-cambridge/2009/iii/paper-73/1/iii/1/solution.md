<h1 id="1/iii/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the proposed exponential profile, put $\ell=u\tau/\phi$. Then $h_x=h/\ell$ and $(hh_x)_x=2h^2/\ell^2$. Thus the exact ratio of the discarded spreading term to the retained advective term is

$$
\boxed{\mathcal E(x,t)=\frac{|u\cot\theta\,(hh_x)_x|}{|uh_x|}=\frac{2\phi h_0\cot\theta}{u\tau}\exp\left[-\frac{t-\phi x/u}{\tau}\right]\ll1.}
$$

This is a quantitative validity condition for the [advection limit of an inclined porous current](../../../../../../../advection-limit-of-an-inclined-porous-current.md). For a specified small tolerance $\eta>0$, at a fixed $x$ it is enough that the inlet characteristic has arrived and

$$
t-\frac{\phi x}{u}>\tau\log\left(\frac{2\phi h_0\cot\theta}{\eta u\tau}\right).
$$

If the logarithm is negative, arrival itself already gives this tolerance. A large-distance estimate comparing the overall current length $ct$ with a height-induced [pressure](../../../../../../../pressure.md) length $h\cot\theta$ is $t\gg\phi h\cot\theta/u$, but the local gradient criterion above is the sharper test for this particular injection history.

At the advective nose, $x=ut/\phi$, the exponential factor is one. Therefore **large time alone is insufficient for uniform validity**: the outer profile also needs $2\phi h_0\cot\theta/(u\tau)\ll1$, and its abrupt nose needs an inner spreading layer. This limitation follows by direct substitution, not from a missing constant in the solution.

Indeed, with $\xi=x-ut/\phi$, the full equation becomes $h_t=D(hh_\xi)_\xi$, $D=u\cot\theta/\phi$. Once a finite-volume injection pulse is effectively over, nonlinear diffusion continues to broaden it. Dimensional balances give width $\ell_d\sim(DMt)^{1/3}$ and height $M/\ell_d$, where $M=\int h\,d\xi$ is the conserved area. A fixed exponential translating profile cannot be the uniform infinite-time limit of that equation. The printed formula is consequently an outer [advection](../../../../../../../advection.md) approximation with the displayed smallness condition.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Iii](../../iii.md)
3. [1](../../../1.md)
4. [Paper 73](../../../../paper-73-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
