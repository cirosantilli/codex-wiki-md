<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $u$ be the actual [displacement field](../../../../../displacement-field-mechanics.md), let $u'$ be an admissible trial [displacement](../../../../../displacement.md), and set $v=u'-u$. On the displacement-prescribed part of the boundary, $v=0$. With actual [stress](../../../../../stress.md) $\sigma=D_\varepsilon W(\varepsilon)$, the supporting-plane inequality for the convex [strain energy density](../../../../../strain-energy-density.md) gives

$$
W(\varepsilon')-W(\varepsilon)\ge\sigma:(\varepsilon'-\varepsilon).
$$

Both $\sigma$ and $\sigma_0$ satisfy [static elastic equilibrium](../../../../../static-elastic-equilibrium.md) with the same [body force](../../../../../body-force.md), so $\nabla\cdot(\sigma-\sigma_0)=0$. On the traction-prescribed boundary their [tractions](../../../../../traction.md) agree. Since $\varepsilon'-\varepsilon=\operatorname{sym}\nabla v$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\int_\Omega(\sigma-\sigma_0):(\varepsilon'-\varepsilon)\,dx
=\int_{\partial\Omega}[(\sigma-\sigma_0)n]\cdot v\,dS=0.
$$

Subtracting the prescribed external-work representative proves the [minimum potential energy principle in elasticity](../../../../../minimum-potential-energy-principle-in-elasticity.md):

$$
\boxed{\int_\Omega\bigl(W(\varepsilon)-\sigma_0:\varepsilon\bigr)\,dx
\le\int_\Omega\bigl(W(\varepsilon')-\sigma_0:\varepsilon'\bigr)\,dx.}
$$

Strict convexity gives uniqueness of the minimizing [strain](../../../../../strain.md), although rigid [displacements](../../../../../displacement.md) can remain when the boundary conditions allow them.

For the comparison bound, put $F(e,x)=W(e,x)-W_0(e)$ and use the [lower conjugate](../../../../../lower-conjugate.md), with its infimum sign convention,

$$
F_*(\tau,x)=\inf_e\{\tau:e-F(e,x)\}.
$$

Its defining inequality is $F_*(\tau,x)\le\tau:e-F(e,x)$, hence $W(e,x)\le W_0(e)+\tau:e-F_*(\tau,x)$ for every $e$. Integrate this pointwise majorant for each compatible [strain](../../../../../strain.md), then take the infimum over the same admissible set. This proves

$$
\boxed{W^{\mathrm{eff}}(E)\le\inf_{e\in K}\int_\Omega
\bigl[W_0(e)+\tau:e-F_*(\tau,x)\bigr],dx.}
$$

No convexity of $F$ is used for this inequality. If $F_*(\tau,x)=-\infty$, it yields only the extended-real upper bound $+\infty$. For example, $W_0=0$ and $W(e)=|e|^2/2$ give $F_*(\tau)=-\infty$ for every finite $\tau$. A useful finite bound requires a suitable comparison energy; choosing a sufficiently stiff quadratic comparison makes the usual excess energies concave. The derivative used below additionally presupposes finite differentiable duals, or an appropriate supergradient formulation.

Now normalize $|\Omega|=1$, take positive constant $C^0$, and write $F_r(e)=W_r(e)-e:C^0e/2$. For phasewise constant [elastic polarization](../../../../../elastic-polarization.md) $\tau=\sum_r\chi_r\tau^r$, its [lower conjugate](../../../../../lower-conjugate.md) contribution is constant within each phase. The remaining minimization is

$$
J_0(E,\tau)=\min_{e\in K}\int_\Omega\left(\tfrac12e:C^0e+\tau:e\right)dx.
$$

Write the minimizing [strain](../../../../../strain.md) as $\widehat e=E+\eta$, where $\eta$ comes from a zero-boundary [displacement field](../../../../../displacement-field-mechanics.md). The [static elastic equilibrium](../../../../../static-elastic-equilibrium.md) equation is $\nabla\cdot(C^0\eta+\tau)=0$, so the supplied [elastic strain Green operator](../../../../../elastic-strain-green-operator.md) gives $\eta=-\Gamma\tau$. Its zero mean removes the cross term with the constant $E$. Using its reciprocity and projection property $\Gamma C^0\Gamma=\Gamma$, we obtain

$$
\begin{aligned}
J_0(E,\tau)
&=\tfrac12E:C^0E+\overline\tau:E
+\tfrac12\langle\Gamma\tau,C^0\Gamma\tau\rangle-\langle\tau,\Gamma\tau\rangle\\
&=\tfrac12E:C^0E+\overline\tau:E-\tfrac12\langle\tau,\Gamma\tau\rangle.
\end{aligned}
$$

Here the brackets in the last two terms denote the spatial integral and [tensor](../../../../../tensor.md) contraction, not just a phase average.

Let $c_r=\int_\Omega\chi_r$. The zero output mean and reciprocity of $\Gamma$ imply that it annihilates constant [elastic polarizations](../../../../../elastic-polarization.md) on either side. Thus subtracting $c_r$ and $c_s$ from the phase indicators does not change their bilinear integral. Define the fourth-order block [tensors](../../../../../tensor.md)

$$
A_{rs}=\int_\Omega\!\int_\Omega
(\chi_r(x)-c_r)\Gamma(x,x')(\chi_s(x')-c_s)\,dx'\,dx.
$$

Consequently $A_{rs}=A_{sr}^T$, $\sum_s A_{rs}=0$, and

$$
\langle\tau,\Gamma\tau\rangle=\sum_{r,s}\tau^r:A_{rs}\tau^s.
$$

These identities follow from reciprocity and $\sum_s\chi_s=\sum_s c_s=1$; no phase independence assumption is needed. The [phase polarization comparison bound](../../../../../phase-polarization-comparison-bound.md), valid for every polarization with finite dual terms, is therefore

$$
\boxed{W^{\mathrm{eff}}(E)\le\mathcal B(E,\tau)
=\tfrac12E:C^0E+\sum_r c_r\tau^r:E
-\tfrac12\sum_{r,s}\tau^r:A_{rs}\tau^s
-\sum_r c_rF_{r*}(\tau^r).}
$$

In particular, it can be optimized over the phase [elastic polarizations](../../../../../elastic-polarization.md) without changing the upper-bound direction.

To derive the final displayed form, impose the stationarity equations in the question. For $c_r>0$, put $e^r=DF_{r*}(\tau^r)$; these are dual [strains](../../../../../strain.md), initially distinct from the comparison solution's phase averages. Reciprocity of $A$ gives

$$
D_{\tau^r}\mathcal B
=c_rE-\sum_sA_{rs}\tau^s-c_re^r.
$$

Thus stationarity is exactly

$$
\boxed{c_re^r+\sum_sA_{rs}\tau^s=c_rE.}
$$

The comparison solution has phase mean

$$
\frac1{c_r}\int_\Omega\chi_r\widehat e\,dx
=E-\frac1{c_r}\sum_sA_{rs}\tau^s,
$$

so **the dual strains become its phase means at stationarity**. Multiplying the stationarity equations by $\tau^r$ and summing gives $\sum_{r,s}\tau^r:A_{rs}\tau^s=\sum_r c_r\tau^r:(E-e^r)$.

For clarity, the [concave biconjugate](../../../../../concave-biconjugate.md) here uses another infimum: $F_{r**}(e)=\inf_s\{s:e-F_{r*}(s)\}$. The [lower conjugate](../../../../../lower-conjugate.md) $F_{r*}$ is concave, since it is an infimum of affine functions. At a differentiable finite point, its supporting-plane inequality shows that $s=\tau^r$ minimizes this last expression when $e=e^r$. Hence

$$
F_{r*}(\tau^r)+F_{r**}(e^r)=\tau^r:e^r.
$$

Substitute both identities into $\mathcal B$ to obtain

$$
\boxed{W^{\mathrm{eff}}(E)\le\tfrac12E:C^0E
+\tfrac12\sum_r c_r\tau^r:(E-e^r)
+\sum_r c_rF_{r**}(e^r).}
$$

This is the requested final bound with the accompanying phase equations. It remains valid at any well-defined stationary choice; asserting existence of such a differentiable choice for arbitrary $W_0$ would require extra hypotheses. Without stationarity, the earlier $\mathcal B(E,\tau)$ is the correct general bound. In the concave closed excess-energy case $F_{r**}=F_r$; for general excess energies replacing the [concave biconjugate](../../../../../concave-biconjugate.md) by $F_r$ without proof would reverse the needed majorant logic.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
