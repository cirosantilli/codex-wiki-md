<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [Einstein-de Sitter universe](../../../../../einstein-de-sitter-universe.md) has $a\propto t^{2/3}$, $H=2/(3t)$, and homogeneous density $\rho=1/(6\pi Gt^2)$. Hence

$$
\boxed{M_i=\frac{4\pi}{3}\rho(t_i)r_i^3=\frac{2r_i^3}{9Gt_i^2}}.
$$

Before the perturbation appreciably changes the motion, every shell follows the [Hubble flow](../../../../../hubble-flow.md),

$$
\boxed{v_i=H_ir_i=\frac{2r_i}{3t_i}}.
$$

By Newton's shell theorem, only matter currently inside a shell contributes to its radial acceleration. Labelling matter by initial radius gives

$$
\boxed{\ddot r(r_i,t)=-\frac{GM(r,t)}{r^2}},
$$



$$
\boxed{M(r,t)=\int_0^\infty
\frac{dM_i}{dr_i}\,
H\!\left(r-r(r_i,t)\right)\,dr_i}.
$$

Before shell crossing, the enclosed mass of a given shell is $M_i$. Its initial specific energy is

$$
E_i=\frac12\left(\frac{2r_i}{3t_i}\right)^2-\frac{GM_i}{r_i}
=-\frac{G\,\delta M_i}{r_i}.
$$

At the [turnaround radius](../../../../../turnaround-radius.md), $E_i=-GM_i/r_*$, so

$$
\boxed{r_*=r_i\frac{M_i}{\delta M_i}}.
$$

The radial Kepler solution from the Big Bang to apocenter gives

$$
\boxed{t_*=\frac\pi2\sqrt{\frac{r_*^3}{2GM_i}}}.
$$

After turnaround a shell falls inward. Shell crossing makes its enclosed mass time dependent; shells then oscillate through the center, form caustics near successive apocenters, and phase mix into a halo.

For [self-similar secondary infall](../../../../../self-similar-secondary-infall.md), write

$$
M(r,t)=M(t)\mathcal M(r/R(t)),\qquad
r(r_i,t)=r_*(r_i)\Lambda(\tau),\qquad
\tau=t/t_*(r_i).
$$

Substitution in the shell equation gives

$$
\frac{r_*}{t_*^2}\Lambda''
=-\frac{GM(t)}{r_*^2\Lambda^2}
\mathcal M\!\left(\frac{r_*\Lambda}{R(t)}\right).
$$

Using $Gt_*^2/r_*^3=\pi^2/(8M_i)$,

$$
\boxed{
\Lambda''(\tau)=
-\frac{\pi^2}{8\Lambda^2}\frac{M(t)}{M_i}
\mathcal M\!\left(\frac{r_*\Lambda}{R(t)}\right)}.
$$

Now impose

$$
\frac{\delta M_i}{M_i}=\left(\frac{M_0}{M_i}\right)^\epsilon.
$$

The case $\epsilon=0$ is a scale-independent fractional overdensity, for which all shells turn around together in the ideal model. The case $\epsilon=1$ has constant excess mass $\delta M_i=M_0$, corresponding to a central point-mass seed outside its core.

Since $r_*/r_i=(M_i/M_0)^\epsilon$, while $r_i^3=(9/2)Gt_i^2M_i$, the turnaround formulas give

$$
\boxed{t_*=\frac{3\pi}{4}t_i
\left(\frac{M_i}{M_0}\right)^{3\epsilon/2}},
$$



$$
\boxed{r_*(M_i)=
\left[\frac8{\pi^2}t_*^2GM_i\right]^{1/3}}.
$$

The shell turning at time $t$ therefore has

$$
\boxed{M(t)=M_0
\left(\frac{4t}{3\pi t_i}\right)^{2/(3\epsilon)}},
$$



$$
\boxed{R(t)=
\left[\frac{8t^2G}{\pi^2}M(t)\right]^{1/3}}.
$$

For a shell with $\tau=t/t_*(M_i)$,

$$
\boxed{\frac{M(t)}{M_i}=\tau^{2/(3\epsilon)}},
\qquad
\boxed{\frac{r_*(M_i)}{R(t)}
=\tau^{-2/3-2/(9\epsilon)}}.
$$

Consequently its autonomous similarity equation is

$$
\boxed{
\Lambda''=
-\frac{\pi^2}{8}\frac{\tau^{2/(3\epsilon)}}{\Lambda^2}
\mathcal M\!\left(
\frac{\Lambda}{\tau^{2/3+2/(9\epsilon)}}
\right)}.
$$

The exponent $2/(3\epsilon)$ follows directly from the preceding mass ratio; the printed $2\epsilon/3$ in the final displayed equation is inconsistent with the supplied initial condition and preceding requested result. The corrected nonlinear equation is integrated numerically after turnaround.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
