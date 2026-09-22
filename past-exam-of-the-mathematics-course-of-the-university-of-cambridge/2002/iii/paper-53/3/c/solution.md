<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the extending direction as $x$ and write $s=\dot\gamma>0$. The [uniaxial extensional flow](../../../../../../uniaxial-extensional-flow.md), satisfying [incompressibility](../../../../../../incompressible-flow.md), has

$$
K=\operatorname{diag}(s,-s/2,-s/2).
$$

Starting from rest, symmetry preserves $A=\operatorname{diag}(a,b,b)$. The [differential pom-pom model](../../../../../../differential-pom-pom-model.md) tensor equation becomes

$$
\dot a=(2s-1/\tau_1)a+1/\tau_1,\qquad
\dot b=-(s+1/\tau_1)b+1/\tau_1,\qquad a(0)=b(0)=1.
$$

Put $x=s\tau_1$. For $x\ne1/2$, the solutions are

$$
a(t)=\frac{1-2x e^{(2x-1)t/\tau_1}}{1-2x},\qquad
b(t)=\frac{1+x e^{-(1+x)t/\tau_1}}{1+x}.
$$

If $x<1/2$, both transients decay, giving

$$
\boxed{A_\infty=\operatorname{diag}\left(\frac1{1-2x},\frac1{1+x},\frac1{1+x}\right).}
$$

If $x>1/2$, the axial component is instead $a=(2x e^{(2x-1)t/\tau_1}-1)/(2x-1)$ and grows exponentially without bound, while $b\to1/(1+x)$. At the boundary $x=1/2$, which lies between the two stated regimes, $a=1+t/\tau_1$ grows linearly and $b\to2/3$.

Normalization makes the molecular orientation finite even when the unnormalized [conformation tensor](../../../../../../conformation-tensor.md) diverges. For $0\le x<1/2$, direct division by $a+2b$ gives

$$
\boxed{B_\infty=\operatorname{diag}\left(\frac{1+x}{3(1-x)},\frac{1-2x}{3(1-x)},\frac{1-2x}{3(1-x)}\right).}
$$

For $x>1/2$, the divergent axial component dominates the [matrix trace](../../../../../../matrix-trace.md), so

$$
\boxed{B_\infty=\operatorname{diag}(1,0,0).}
$$

The same normalized limit holds at $x=1/2$, agreeing continuously with the limit of the subcritical expression. The limiting orientations have nonnegative [eigenvalues](../../../../../../eigenvalue.md) and unit [matrix trace](../../../../../../matrix-trace.md), as required for the normalized molecular orientation.

Now set $S(t)=B(t):K=s(a-b)/(a+2b)$. Its limiting value is

$$
S_\infty(s)=\begin{cases}
s^2\tau_1/(1-s\tau_1),&s\tau_1<1/2,\\
s,&s\tau_1\ge1/2.
\end{cases}
$$

The [scalar](../../../../../../scalar.md) stretch equation is $\dot\lambda=[S(t)-1/\tau_2]\lambda+1/\tau_2$. If $S_\infty<1/\tau_2$, its coefficient is eventually bounded above by a negative constant. The [variation of constants](../../../../../../variation-of-parameters.md) formula gives a bounded solution, converging to

$$
\lambda_\infty=\frac1{1-\tau_2S_\infty}.
$$

If $S_\infty>1/\tau_2$, the coefficient is eventually positive, and the positive stretch grows without bound. At equality a bounded stretch would imply $\dot\lambda\to1/\tau_2>0$, which contradicts boundedness. Thus equality is not an additional bounded steady regime.

The function $S_\infty(s)$ is continuous and strictly increasing from zero to infinity. Consequently there is a unique critical extension rate defined by

$$
\tau_2 S_\infty(\dot\gamma_c)=1,
$$

and **the molecular stretch remains bounded precisely for $\dot\gamma<\dot\gamma_c$**. This is distinct from the tensor threshold $\dot\gamma\tau_1=1/2$. If $\tau_2<2\tau_1$, for example, the normalized orientation can remain well defined and the stretch remain bounded for some rates above the tensor threshold; divergence of $A$ alone does not prove divergence of the physical [stress](../../../../../../stress.md).

In the requested doubly subcritical regime, write $D=1-s\tau_1-s^2\tau_1\tau_2>0$. The [steady uniaxial extension of the differential pom-pom model](../../../../../../steady-uniaxial-extension-of-the-differential-pom-pom-model.md) has

$$
\lambda_\infty=\frac{1-s\tau_1}{D},\qquad
B_{xx,\infty}-B_{yy,\infty}=\frac{s\tau_1}{1-s\tau_1}.
$$

The isotropic [pressure](../../../../../../pressure.md) cancels from the tensile [normal-stress difference](../../../../../../normal-stress-difference.md). Hence the [extensional viscosity](../../../../../../extensional-viscosity.md) is

$$
\eta_E=\frac{\sigma_{xx}-\sigma_{yy}}s
=\frac{G\lambda_\infty^2}{s}(B_{xx,\infty}-B_{yy,\infty}),
$$

or

$$
\boxed{\eta_E(s)=\frac{G\tau_1(1-s\tau_1)}{(1-s\tau_1-s^2\tau_1\tau_2)^2},\qquad
s\tau_1<\frac12,\quad s<\dot\gamma_c.}
$$

Its zero-rate limit is $G\tau_1=3\mu_0$, recovering the [Trouton ratio](../../../../../../trouton-ratio.md) of three. The restrictions exclude both loss of a finite tensor steady state and loss of a finite stretch steady state; neither denominator may be continued through its singularity as a physical steady constitutive response.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
