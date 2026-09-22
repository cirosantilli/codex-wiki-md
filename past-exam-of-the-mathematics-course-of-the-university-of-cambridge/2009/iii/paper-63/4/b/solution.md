<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To obtain the specified expansion, use the usual nova-ejection prescription: the escaping material is expelled isotropically from the [white dwarf](../../../../../../white-dwarf.md) and carries its specific orbital [angular momentum](../../../../../../angular-momentum.md), with no additional [torque](../../../../../../torque.md). This is [isotropic re-emission from a binary star](../../../../../../isotropic-re-emission-from-a-binary-star.md). Circularity alone does not determine the [angular momentum](../../../../../../angular-momentum.md) carried by the ejecta; the prescription is an additional physical assumption.

The accretor's orbital radius is $a_1=aM_2/M$, so its [specific angular momentum](../../../../../../specific-angular-momentum.md) satisfies

$$
j_1=a_1^2\Omega,\qquad \frac{j_1}{J}=\frac{M_2}{M_1M}=\frac qM.
$$

During ejection, take $\delta M_1=-\delta m$, $\delta M_2=0$ and $\delta M=-\delta m$, where $\delta m>0$. Consequently

$$
\frac{\delta J}J=-\frac{q\delta m}{M}.
$$

Differentiate $J=M_1M_2\sqrt{Ga/M}$ to first order:

$$
-\frac{q\delta m}{M}
=-\frac{\delta m}{M_1}+\frac12\frac{\delta a}a+\frac12\frac{\delta m}{M}.
$$

Using $M/M_1=1+q$ yields

$$
\boxed{\frac{\delta a}a=\frac{\delta m}{M}.}
$$

The same lobe law now has changing total [mass](../../../../../../mass.md) but unchanged donor [mass](../../../../../../mass.md), so

$$
\boxed{\frac{\delta R_L}{R_L}
=\frac{\delta a}a+\frac13\left(\frac{\delta M_2}{M_2}-\frac{\delta M}{M}\right)
=\frac{4\delta m}{3M}.}
$$

The donor radius is unchanged on the short eruption timescale, whereas its lobe expands. It therefore falls inside the lobe and [Roche-lobe overflow](../../../../../../roche-lobe-overflow.md) stops in this idealized model. This is [nova-induced binary detachment](../../../../../../nova-induced-binary-detachment.md).

The need for the ejection prescription can also be seen algebraically. If the ejecta instead have mean [specific angular momentum](../../../../../../specific-angular-momentum.md) $j_{\mathrm{ej}}=\eta_JJ/M$, the same circular-orbit differentiation gives

$$
\frac{\delta a}a=(1+2q-2\eta_J)\frac{\delta m}{M}.
$$

The requested coefficient is obtained only when $\eta_J=q$. Other prescriptions can produce a different expansion or a contraction; the stated circularity condition does not rule them out. The ejection may be short compared with the transfer time while remaining slow compared with an orbit, consistent with circularity. If truly impulsive, an eccentricity is generally excited unless an additional circularization assumption is made.

Now put $\Gamma=-\dot J>0$ for the constant external [torque](../../../../../../torque.md). Keep the masses, [mass](../../../../../../mass.md) ratio and [torque](../../../../../../torque.md) coefficients fixed to leading order over one small-$\delta m$ cycle; corrections in those coefficients affect the calculated times only at the next order. During detachment there is no transfer, so fixed component masses give

$$
\frac{\dot R_L}{R_L}=\frac{\dot a}a=-\frac{2\Gamma}{J}.
$$

The fractional lobe gap $4\delta m/(3M)$ closes in time

$$
\boxed{t_d=\frac{2J\delta m}{3M\Gamma}.}
$$

During the semi-detached accumulation phase, use the same external [torque](../../../../../../torque.md) and the equilibrium donor contact equation derived in (a):

$$
-\dot M_2=\dot M_1=\frac{3\Gamma M_2}{J(4-3q)}.
$$

Accumulating the next layer therefore takes

$$
\boxed{t_s=\frac{J\delta m(4-3q)}{3\Gamma M_2}.}
$$

Division cancels the layer [mass](../../../../../../mass.md), [torque](../../../../../../torque.md) and [angular momentum](../../../../../../angular-momentum.md):

$$
\boxed{\frac{t_d}{t_s}=\frac{2M_2}{M(4-3q)}
=\frac{2q}{(4-3q)(1+q)}.}
$$

The result uses $q<4/3$ for a positive steady accumulation rate, unchanged donor structure during the eruption and the same external [torque](../../../../../../torque.md) in the two phases. Here the given $q<1$ ensures a positive denominator. It describes an idealized nova cycle; extra frictional loss, irradiation-driven donor changes or a different ejection [angular momentum](../../../../../../angular-momentum.md) would change the ratio.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
