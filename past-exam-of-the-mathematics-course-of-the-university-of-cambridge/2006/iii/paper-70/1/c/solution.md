<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $a=v_2/v_1$. Mass and normal [momentum conservation](../../../../../../momentum-conservation.md) imply

$$
\rho_2=\rho_1/a,\qquad p_2=p_1+\rho_1v_1^2(1-a).
$$

After cancelling the unchanged tangential kinetic energies, the energy condition is $v_1^2/2+\gamma p_1/[(\gamma-1)\rho_1]=a^2v_1^2/2+\gamma a p_2/[(\gamma-1)\rho_1]$. With $v_{s1}^2=\gamma p_1/\rho_1$ and normal [Mach number](../../../../../../mach-number.md) $\mathcal M=v_1/v_{s1}$, rearrangement factors it as

$$
(1-a)\left[(\gamma-1)+\frac2{\mathcal M^2}-(\gamma+1)a\right]=0.
$$

The first root is the no-shock solution. The nontrivial [perfect-gas shock jump conditions](../../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md) therefore give

$$
\boxed{\frac{u_{x2}}{u_{x1}}=
\frac{(\gamma-1)\mathcal M^2+2}{(\gamma+1)\mathcal M^2}.}
$$

Its [density](../../../../../../density.md) and [pressure](../../../../../../pressure.md) ratios are

$$
\frac{\rho_2}{\rho_1}=\frac{(\gamma+1)\mathcal M^2}{(\gamma-1)\mathcal M^2+2},\qquad
\frac{p_2}{p_1}=\frac{2\gamma\mathcal M^2-(\gamma-1)}{\gamma+1}.
$$

Physical admissibility selects a compressive, entropy-increasing shock. This can be verified directly: with $X=\mathcal M^2$, define $K_i=p_i/\rho_i^\gamma$. The derivative of $\ln(K_2/K_1)$ after inserting these ratios is

$$
\frac{d}{dX}\ln\frac{K_2}{K_1}
=\frac{2\gamma(\gamma-1)(X-1)^2}
{[2\gamma X-(\gamma-1)]X[(\gamma-1)X+2]}>0\quad(X\ne1),
$$

where pressures are positive, and $K_2/K_1=1$ at $X=1$. Thus the [entropy](../../../../../../entropy.md) increases precisely on the branch $X>1$; the positive-pressure expansion branch $X<1$ decreases [entropy](../../../../../../entropy.md). Since the normal speed is positive,

$$
\boxed{1<\mathcal M<\infty.}
$$

The endpoint one is the zero-strength limit, not a finite shock. The downstream normal [Mach number](../../../../../../mach-number.md) obeys $\mathcal M_2^2=[(\gamma-1)\mathcal M^2+2]/[2\gamma\mathcal M^2-(\gamma-1)]<1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
