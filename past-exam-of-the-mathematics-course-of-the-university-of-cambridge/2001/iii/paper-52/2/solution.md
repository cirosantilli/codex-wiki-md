<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $q_i>0$ measure the relative trapping vulnerability and use fixed species-specific catches $q_iH$. With no natural interaction, the two populations satisfy independent [constant-quota harvested logistic growth](../../../../../constant-quota-harvested-logistic-growth.md) equations,

$$
\dot N_i=r_iN_i\left(1-\frac{N_i}{K_i}\right)-q_iH,
\qquad i=1,2.
$$

This treats $H$ as a common harvest scale: a total fixed quota can equivalently be allocated in fixed fractions $q_1+q_2=1$. Catches are not reassigned after one species disappears. [Carrying capacity](../../../../../carrying-capacity.md) and intrinsic growth differ between species; greater trapping vulnerability alone therefore does not determine which species disappears first.

The maximum natural surplus occurs at $N_i=K_i/2$. Define the critical harvesting level

$$
\boxed{H_{c,i}=\frac{r_iK_i}{4q_i}.}
$$

For $0<H<H_{c,i}$ there are two positive [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md),

$$
\boxed{N_{i,\pm}=\frac{K_i}{2}
\left(1\pm\sqrt{1-H/H_{c,i}}\right).}
$$

The [derivative](../../../../../derivative.md) of the population vector field is negative at the upper branch and positive at the lower branch. The upper branch is attracting; the lower is an unstable survival threshold. An initial abundance above the lower branch approaches the upper branch, whereas one below it reaches extinction. At $H=0$, positive populations approach $K_i$, while zero remains zero.

At $H=H_{c,i}$ the branches meet in a [saddle-node bifurcation](../../../../../saddle-node-bifurcation.md) and

$$
\dot N_i=-\frac{r_i}{K_i}(N_i-K_i/2)^2.
$$

Initial abundances above $K_i/2$ approach it algebraically from above; those below decline to extinction. For $H>H_{c,i}$ there is no positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) and the [derivative](../../../../../derivative.md) of abundance is everywhere negative. In fact $\dot N_i\le-q_i(H-H_{c,i})$, giving finite extinction time. At zero the biological model stops harvesting and keeps the population extinct rather than extending the constant-quota equation to negative abundance.

Order the thresholds as $H_{c,1}<H_{c,2}$. Below the first threshold, both species can persist if each starts above its own survival threshold; either or both can still disappear from inadequate initial abundance. Between the thresholds only species 2 can persist. Above the second, neither can persist. At each threshold use the one-sided critical behaviour just derived. Equal thresholds give simultaneous loss of both positive branches. Because the equations are independent, there are no sustained oscillations or competitive replacements in this model.

<a id="2/image-stable-and-unstable-equilibrium-branches-of-two-independently-harvested-logistic-populations"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-52-harvest-equilibria.png)

**[Figure 2](#2/image-stable-and-unstable-equilibrium-branches-of-two-independently-harvested-logistic-populations). Stable and unstable equilibrium branches of two independently harvested logistic populations**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
