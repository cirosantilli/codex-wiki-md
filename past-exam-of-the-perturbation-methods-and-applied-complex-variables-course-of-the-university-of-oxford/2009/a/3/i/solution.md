<h1 id="a/3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose $\delta=\sqrt\epsilon$ in the [WKB approximation](../../../../../wkb-approximation.md) and substitute $y=\exp(S_0/\delta+S_1+\cdots)$. The leading equation is

$$
(S_0')^2=x,
$$

so take $S_0=\pm2x^{3/2}/3$. At the next order,

$$
2S_0'S_1'+S_0''+(x-1)S_0'=0,
$$

giving

$$
S_1=-\tfrac14\log x-\tfrac14x^2+\tfrac12x
$$

up to an absorbed constant. Label the recessive and dominant branches respectively by

$$
y_1=x^{-1/4}e^{-x^2/4+x/2}e^{-2x^{3/2}/(3\sqrt\epsilon)},\qquad
y_2=x^{-1/4}e^{-x^2/4+x/2}e^{2x^{3/2}/(3\sqrt\epsilon)}.
$$

The formal outer solution is $c_1y_1+c_2y_2$. The point zero is a simple [wave turning point](../../../../../wave-turning-point.md): $S_0'$ vanishes and the WKB amplitude diverges.

The boundary condition at infinity selects **$c_2=0$**, with $c_1$ to be fixed by matching. This statement concerns the actual recessive branch. One cannot literally send $x\to\infty$ in the truncated small-$\epsilon$ formulas: their ordering fails when $\epsilon x$ is no longer small, and their common Gaussian factor would then spuriously suggest that both branches decay.

To justify the selection, remove the first derivative exactly with $y=e^{-x^2/4+x/2}v$. Then

$$
v''=\left[\frac x\epsilon+\frac{(x-1)^2}4+\frac12\right]v.
$$

The coefficient is positive for $x\geq0$, so it has distinct dominant and recessive branches. For very large $x$, the dominant branch restores $y$ growth of exponential rate $1/\epsilon$, while the recessive branch decays. Matching to this recessive branch removes $c_2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
