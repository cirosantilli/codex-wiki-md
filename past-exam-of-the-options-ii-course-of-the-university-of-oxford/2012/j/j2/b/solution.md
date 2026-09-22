<h1 id="j/j2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The Born [probability](../../../../../probability.md) is the [integral](../../../../../integral-split.md) of $|\psi_n|^2$ over the indicated [interval](../../../../../interval-mathematics.md). Changing variables to $\xi$ cancels the dimensional [normalization](../../../../../normalization.md) factors and gives

$$
P_0(\ell)=\frac1{\sqrt\pi}\int_{-\ell}^{\ell}e^{-\xi^2}\,d\xi,\qquad
P_1(\ell)=\frac2{\sqrt\pi}\int_{-\ell}^{\ell}\xi^2e^{-\xi^2}\,d\xi.
$$

Since $\frac{d}{d\xi}(\xi e^{-\xi^2})=e^{-\xi^2}-2\xi^2e^{-\xi^2}$, integration gives

$$
\boxed{P_1(\ell)=P_0(\ell)-\frac2{\sqrt\pi}\ell e^{-\ell^2}.}
$$

As $\ell\to\infty$, the correction term tends to zero and $P_0(\ell)\to1$ by [normalization](../../../../../normalization.md). Hence $\boxed{P_1(\ell)\to1}$. This is expected because the expanding [interval](../../../../../interval-mathematics.md) exhausts the whole position space and the state is normalized: the particle is somewhere on the [line](../../../../../straight-line.md) with total [probability](../../../../../probability.md) one.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [J2](../../j2.md)
3. [J](../../../j.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
