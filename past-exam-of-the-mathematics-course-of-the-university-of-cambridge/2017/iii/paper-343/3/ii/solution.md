<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a spatially uniform pump and $\beta>0$, a nonzero homogeneous solution has constant [number density](../../../../../../number-density.md) determined by gain saturation. Its [complex argument](../../../../../../argument-complex-analysis.md) rotates uniformly:

$$
\boxed{\Psi_\infty(t)=\sqrt{n_\infty}\,e^{-i\mu t+i\theta_0},\qquad
n_\infty=\frac\alpha\beta,\qquad \mu=gn_\infty-s.}
$$

This [uniform pumped polariton condensate](../../../../../../uniform-pumped-polariton-condensate.md) requires $\alpha>0$, equivalently

$$
P>P_{\rm th}=\frac{\gamma_C\gamma_R}{R_R}.
$$

In the cubic approximation its [number density](../../../../../../number-density.md) is

$$
n_\infty=\frac{\gamma_R}{R_R}\left(1-\frac{P_{\rm th}}P\right).
$$

It is not the exact [number density](../../../../../../number-density.md) of the original two-field equations, which would be $(P-P_{\rm th})/\gamma_C$: the two coincide to first order in distance above threshold. At or below threshold there is no positive nonzero branch of this form; the vacuum remains a solution. This algebra establishes existence, not stability for every possible sign of $g$.

Choose $\theta_0=0$ and seek a time-independent normalized profile through

$$
\Psi(\mathbf r,t)=\sqrt{n_\infty}\,e^{-i\mu t}\psi(\mathbf r).
$$

Using $\beta n_\infty=\alpha$ and $\mu+s=gn_\infty$, its equation becomes

$$
0=\alpha(1-|\psi|^2)\psi+i\left[\nabla^2+gn_\infty(1-|\psi|^2)\right]\psi.
$$

Division by $i$ therefore yields

$$
\boxed{\left[\nabla^2+\xi(1-|\psi|^2)\right]\psi=0,\qquad
\xi=(g-i\beta)n_\infty=gn_\infty-i\alpha.}
$$

For a localized zero-winding disturbance the bulk condition is $\psi\to1$. Here $\xi$ is a complex coefficient with inverse-length-squared dimensions in the scaled equation, not the real wall-healing length denoted by the same letter in Question 1. The [constant far-field phase excludes net vortex winding](../../../../../../constant-far-field-phase-excludes-net-vortex-winding.md) lemma explains why the next part requires interpreting the vortex boundary differently.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
