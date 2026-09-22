<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Two event-time distributions form an [accelerated life family](../../../../../accelerated-life-family.md) if one is a positive time rescaling of the other: $S_1(t)=S_0(t/k)$ for some $k>0$. They form a [proportional hazards family](../../../../../proportional-hazards-family.md) if their [hazard functions](../../../../../hazard-function.md) satisfy $h_1(t)=r h_0(t)$ for a constant $r>0$, equivalently $S_1(t)=S_0(t)^r$ for continuous distributions.

First take the standard positive-scale convention $c>0$. Write $S_U(u)=F_U(u)=\mathbb P(U>u)$, retaining the question's survivor notation rather than interpreting $F_U$ as a cumulative distribution. Since $T_z=e^{a+bz}U^c$,

$$
\boxed{S_z(t)=S_U\left(t^{1/c}e^{-(a+bz)/c}\right),\qquad t>0.}
$$

It follows that $S_z(t)=S_0(te^{-bz})$, proving the [accelerated life family](../../../../../accelerated-life-family.md) property with time multiplier $e^{bz}$. In fact the scaling identity $T_z\overset d=e^{bz}T_0$ holds for any fixed real $c$.

The given density integrates to $\mathbb P(X\leq x)=1-e^{-e^x}$, so $U=e^X$ has the unit [exponential distribution](../../../../../exponential-distribution.md). Its survivor is $e^{-u}$. Consequently

$$
S_z(t)=\exp\left[-e^{-(a+bz)/c}t^{1/c}\right],\qquad
h_z(t)=\frac1c e^{-(a+bz)/c}t^{1/c-1},
$$

and

$$
\boxed{h_z(t)/h_0(t)=e^{-bz/c}.}
$$

These are the [Weibull accelerated-life and proportional-hazards families](../../../../../weibull-accelerated-life-and-proportional-hazards-families.md), with common shape $1/c>0$.

The positive-scale assumption is necessary for this last conclusion and is not explicit in the printed description of the constants. If $c<0$, the transformation reverses the inequality, giving $S_z(t)=1-S_U(r-)$ with $r=t^{1/c}e^{-(a+bz)/c}$; for continuous $U$ this is $1-S_U(r)$. For the given density these are scaled [Fréchet distributions](../../../../../frechet-distribution.md), generally not proportional hazards. The [negative log-scale counterexample to proportional hazards](../../../../../negative-log-scale-counterexample-to-proportional-hazards.md) uses $a=0,c=-1,b=\log2$ and has hazard ratio $2/(e^{1/t}+1)$, which depends on time. If $c=0$, $T_z=e^{a+bz}$ is deterministic, with survivor $\mathbf1_{\{t<e^{a+bz}\}}$, so an ordinary density-based hazard does not apply. These cases preserve the accelerated-life identity but do not prove the asserted proportional-hazards conclusion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
