<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $\hbar=c=1$ in the field-theory calculations. Work with signature $(+,-)$ and $a\ne0$. Since $x=(x_++x_-)$ and $t=(x_+-x_-)$, $\partial_+=\partial_x+\partial_t$, $\partial_-=\partial_x-\partial_t$, and the [Sine-Gordon equation](../../../../../sine-gordon-equation.md) is $\phi_{+-}=\sin\phi$. Introduce $w=(\rho+\kappa)/2$ and $d=(\rho-\kappa)/2$. The specified [Sine-Gordon Bäcklund transformation](../../../../../sine-gordon-backlund-transformation.md) becomes $d_+=a\sin w$, $w_-=a^{-1}\sin d$. Its compatibility gives

$$
d_{+-}=\cos w\sin d,\qquad w_{+-}=\cos d\sin w.
$$

Adding and subtracting these equations establishes

$$
\boxed{\rho_{+-}=\sin(w+d)=\sin\rho,\qquad \kappa_{+-}=\sin(w-d)=\sin\kappa.}
$$

Thus a compatible transformed field satisfies the same [Sine-Gordon equation](../../../../../sine-gordon-equation.md). Smoothness is needed to interchange mixed derivatives. The statement cannot literally include $a=0$, since one defining equation contains $1/a$.

**Generating the [kink](../../../../../scalar-field-kink.md).** With zero seed, the two first-order equations give $\rho_+=2a\sin(\rho/2)$ and $\rho_-=2a^{-1}\sin(\rho/2)$. On a nonconstant branch put $p=\tan(\rho/4)$; then $p_+=ap$, $p_-=a^{-1}p$. Integration gives

$$
\boxed{\rho=4\arctan\left[C\exp\left(\tfrac12(a+a^{-1})x+\tfrac12(a-a^{-1})t\right)\right].}
$$

For $a>0,C>0$, this is the [Sine-Gordon kink](../../../../../sine-gordon-kink.md), after absorbing $C$ in the center position. Its speed and Lorentz factor obey

$$
\boxed{v=\frac{1-a^2}{1+a^2},\qquad (1-v^2)^{-1/2}=\tfrac12(a+a^{-1}),\qquad a=e^{-\eta},\ v=\tanh\eta.}
$$

Changing the sign of $a$ or of the exponential coefficient selects the corresponding [antikink](../../../../../antikink.md) orientation; $|v|<1$ whenever $a$ is finite and nonzero. Constant vacuum branches, omitted by division by $\sin(\rho/2)$, can be added separately.

The continuously parametrized [Bäcklund transformation](../../../../../backlund-transformation.md) does more than produce this one solution. Successive compatible transformations and [Bianchi permutability for sine-Gordon Bäcklund transformations](../../../../../bianchi-permutability-for-sine-gordon-backlund-transformations.md) construct [multisoliton solutions](../../../../../multisoliton-solution.md); expansion of the generating relations gives the [local conserved-charge hierarchy of sine-Gordon theory](../../../../../local-conserved-charge-hierarchy-of-sine-gordon-theory.md). Together with its [Lax pair](../../../../../lax-pair.md) and [inverse scattering transform](../../../../../inverse-scattering-transform.md), this is the structure behind [classical integrability](../../../../../classical-integrability.md), elastic scattering and the absence of generic radiative energy loss in [soliton](../../../../../soliton.md) collisions. Existence of a transformation alone is not a proof that every generated [conserved charge](../../../../../conserved-charge.md) is independent and in involution; those are additional properties of the integrable system.

**Transforming the static [kink](../../../../../scalar-field-kink.md) at $a=1$.** The seed obeys $\kappa_x=2\operatorname{sech}x$, $\sin(\kappa/2)=\operatorname{sech}x$, $\cos(\kappa/2)=-\tanh x$. Adding and subtracting the two [Sine-Gordon Bäcklund transformation](../../../../../sine-gordon-backlund-transformation.md) equations yields

$$
\rho_x=-2\tanh x\sin(\rho/2),\qquad \rho_t=2\operatorname{sech}x[1+\cos(\rho/2)].
$$

Again set $p=\tan(\rho/4)$. These simplify to $p_x=-p\tanh x$, $p_t=\operatorname{sech}x$. The first gives $p=f(t)/\cosh x$, and the second gives $f'=1$. Therefore

$$
\boxed{\rho(x,t)=4\arctan\frac{t-t_0}{\cosh x}.}
$$

Continuous inverse-tangent branches may be chosen without creating artificial jumps. At spatial infinity the field approaches the same vacuum, so its net [topological charge](../../../../../topological-charge.md) is zero. For large $|t-t_0|$ there are two well-separated transitions near $x_\pm=\pm\operatorname{arcosh}|t-t_0|$, with speeds tending to zero. The two transitions exchange their [kink](../../../../../scalar-field-kink.md)/[antikink](../../../../../antikink.md) orientations as they pass through the collision, while the field remains smooth.

This is the [Sine-Gordon threshold kink-antikink solution](../../../../../sine-gordon-threshold-kink-antikink-solution.md), a [separatrix](../../../../../separatrix.md) between finite-speed scattering and the bounded [Sine-Gordon breather](../../../../../sine-gordon-breather.md) motion, rather than a finite-period breather. In fact it is the $v\to0$ limit of the scattering field in question 3. At $t=t_0$, $\rho=0$ and $\rho_t=4\operatorname{sech}x$, so the reduced energy is $\int\rho_t^2dx/2=16$, exactly twice the reduced single-kink energy $8$.

For [mass](../../../../../mass.md) comparisons below, the original PDF really prints $m^2/\beta$. Restoring physical coordinates $X=x/m$, $T=t/m$ gives the angular-field action $\beta^{-1}\int dtdx[\tfrac12(\partial\phi)^2+\cos\phi-1]$ and literal [kink](../../../../../scalar-field-kink.md) [mass](../../../../../mass.md) $8m/\beta$, for $\beta>0$. The usual [Sine-Gordon theory](../../../../../sine-gordon-theory.md) instead has prefactor $m^2/\beta^2$ and [mass](../../../../../mass.md) $8m/\beta^2$. The equation of motion and every field above are unchanged by this overall normalization; the quantum scattering comparison in question 3 is not.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
