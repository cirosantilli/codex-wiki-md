<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [Voigt elastic approximation](../../../../../../voigt-elastic-approximation.md), every local [strain](../../../../../../strain.md) is $E$. The corresponding local [stress](../../../../../../stress.md) is $\sigma_V(x)=D_\varepsilon W(E,x)$. Differentiating the averaged [strain energy density](../../../../../../strain-energy-density.md) under the integral gives

$$
\boxed{DW_V(E)=\langle D_\varepsilon W(E,x)\rangle=\langle\sigma_V\rangle.}
$$

The uniform [strain](../../../../../../strain.md) need not generate an equilibrated local [stress](../../../../../../stress.md); this calculation concerns the stated approximation, not an assertion that it solves the heterogeneous boundary problem.

For the [Reuss elastic approximation](../../../../../../reuss-elastic-approximation.md), use the [convex conjugate](../../../../../../convex-conjugate.md)

$$
W^*(S,x)=\sup_e\{S:e-W(e,x)\}.
$$

Under differentiable strictly convex duality, the local [strain](../../../../../../strain.md) produced by uniform [stress](../../../../../../stress.md) $S$ is $e_R(x)=D_SW^*(S,x)$. Set $F(S)=\langle W^*(S,x)\rangle$. Averaging the local [strains](../../../../../../strain.md) gives $E=DF(S)$. At the maximizing [stress](../../../../../../stress.md) in $W_R(E)=F^*(E)$, the stationarity condition is precisely $DF(S)=E$. Consequently

$$
\begin{aligned}
DW_R(E):H
&=D_E\bigl(S(E):E-F(S(E))\bigr):H\\
&=S:H+DS(E)[H]:\bigl(E-DF(S)\bigr)=S:H.
\end{aligned}
$$

Thus **the derivative of each approximate energy is its own mean stress**, including

$$
\boxed{DW_R(E)=S=\langle\sigma_R\rangle.}
$$

For positive [linear elasticity](../../../../../../linear-elasticity.md), $W=e:C(x)e/2$ and $W^*=S:C(x)^{-1}S/2$, giving the useful check $C_V=\langle C\rangle$ and $C_R=\langle C^{-1}\rangle^{-1}$. More general convex duality gives the same conjugacy relation with [subgradients](../../../../../../subgradient.md) when differentiability or strict convexity is absent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
