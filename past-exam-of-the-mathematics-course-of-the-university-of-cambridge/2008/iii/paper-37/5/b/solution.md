<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work on a common stochastic basis on which $B,B'$ are independent [Brownian motions](../../../../../../brownian-motion-split.md) and the solutions are adapted; independent weak solutions can be put on the product stochastic basis. Independence gives $[B,B']=0$. Put $S=Z+Z'\geq0$ and define the predictable weights

$$
u_t=\begin{cases}\sqrt{Z_t/S_t},&S_t>0,\\1,&S_t=0,\end{cases}\qquad
v_t=\begin{cases}\sqrt{Z'_t/S_t},&S_t>0,\\0,&S_t=0.\end{cases}
$$

They are bounded and satisfy $u_t^2+v_t^2=1$ everywhere. Define

$$
\boxed{\beta_t=\int_0^tu_s\,dB_s+\int_0^tv_s\,dB'_s.}
$$

This is a zero-start [continuous local martingale](../../../../../../continuous-local-martingale.md), and its [quadratic variation](../../../../../../quadratic-variation.md) is $[\beta]_t=\int_0^t(u_s^2+v_s^2)ds=t$. By the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md), $\beta$ is a [Brownian motion](../../../../../../brownian-motion-split.md) in the common filtration.

On $\{S_t>0\}$, $\sqrt{S_t}u_t=\sqrt{Z_t}$ and $\sqrt{S_t}v_t=\sqrt{Z'_t}$. On $\{S_t=0\}$, nonnegativity forces both $Z_t,Z'_t$ to be zero, so the same identities hold. [Associativity of stochastic integration](../../../../../../associativity-of-stochastic-integration.md) therefore gives

$$
S_t=z+z'+\int_0^t\sqrt{S_s}\,d\beta_s.
$$

This proves the [addition law for square-root branching diffusions](../../../../../../addition-law-for-square-root-branching-diffusions.md): **$Z+Z'$ is a weak solution with initial value $z+z'$**. Specifying the weights at zero is necessary to keep $[\beta]_t=t$ after extinction; simply setting both weights to zero would fail to produce a Brownian driver.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
