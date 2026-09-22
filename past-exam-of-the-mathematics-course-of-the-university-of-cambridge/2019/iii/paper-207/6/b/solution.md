<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
m=\pi\gamma+(1-\pi)\beta,
$$

and use constant baseline hazard $h_0=m$. Define the two-point frailty

$$
U=
\begin{cases}
\gamma/m,&\text{with probability }\pi,\\
\beta/m,&\text{with probability }1-\pi.
\end{cases}
$$

Then $\mathbb EU=1$, and the conditional rates are exactly $\gamma$ and $\beta$. The experimental-treatment population has

$$
S_E(t)=\pi e^{-\gamma t}+(1-\pi)e^{-\beta t}
$$

and

$$
h_E(t)=
\frac{\pi\gamma e^{-\gamma t}+(1-\pi)\beta e^{-\beta t}}
{\pi e^{-\gamma t}+(1-\pi)e^{-\beta t}}.
$$

Since standard treatment has hazard $\beta$, the population hazard ratio is

$$
\boxed{
R(t)=\frac{h_E(t)}\beta
=\frac{\pi\gamma e^{-\gamma t}+(1-\pi)\beta e^{-\beta t}}
{\beta\{\pi e^{-\gamma t}+(1-\pi)e^{-\beta t}\}}.}
$$

At zero,

$$
R(0)=1-\pi\left(1-\frac\gamma\beta\right),
$$

whereas for $\pi>0$,

$$
R(t)\longrightarrow\frac\gamma\beta
\qquad(t\to\infty).
$$

The treatment effect is therefore non-proportional and strengthens among later survivors as the high-rate subgroup is depleted. A trial should allow adequate follow-up, avoid relying only on a constant-hazard-ratio Cox model, and prespecify survival-curve, milestone-risk, restricted-mean-survival, or time-varying-effect analyses. Its power and interpretation will depend materially on follow-up duration.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
