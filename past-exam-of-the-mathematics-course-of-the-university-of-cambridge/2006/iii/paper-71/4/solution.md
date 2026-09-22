<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $M=M_1+M_2$. The [centre of mass](../../../../../center-of-mass.md) condition gives $a_1=aM_2/M$, $a_2=aM_1/M$. For [circular motion](../../../../../circular-motion.md) the component [angular momenta](../../../../../angular-momentum.md) are $J_i=M_ia_i^2\Omega$, so

$$
J=(M_1a_1^2+M_2a_2^2)\Omega
=\frac{M_1M_2}{M}a^2\Omega.
$$

Using [Kepler's third law](../../../../../kepler-s-third-law.md), $a^3\Omega^2=GM$, and $\Omega=2\pi/P_{\rm orb}$ gives

$$
\boxed{J=\frac{M_1M_2}{M}a^2\Omega
=\frac{G^{2/3}P_{\rm orb}^{1/3}M_1M_2}{(2\pi)^{1/3}M^{1/3}}.}
$$

This is the [circular-binary orbital angular momentum](../../../../../circular-binary-orbital-angular-momentum.md). [Mass](../../../../../mass.md) received by the companion redistributes [angular momentum](../../../../../angular-momentum.md) within the [binary star](../../../../../binary-star.md); only the escaping [stellar wind](../../../../../stellar-wind.md) removes it under the prescribed model.

The [stellar wind](../../../../../stellar-wind.md) from the [donor star](../../../../../donor-star.md) has [specific angular momentum](../../../../../specific-angular-momentum.md)

$$
j_w=\frac{J_1}{M_1}=a_1^2\Omega,\qquad\frac{j_w}{J}=\frac{M_2}{M_1M}.
$$

Here $\dot M_1<0$, $\dot M_2=-f\dot M_1$ and $\dot M=(1-f)\dot M_1$. Thus [donor-wind angular-momentum loss](../../../../../donor-wind-angular-momentum-loss.md) gives

$$
\frac{\dot J}{J}=(1-f)\dot M_1\frac{M_2}{M_1M}.
$$

Taking the [logarithmic derivative](../../../../../logarithmic-derivative.md) of the period expression for $J$ gives

$$
\frac{\dot P_{\rm orb}}{P_{\rm orb}}
=3\frac{\dot J}{J}-3\frac{\dot M_1}{M_1}-3\frac{\dot M_2}{M_2}+\frac{\dot M}{M}.
$$

Use $M_2/(M_1M)=1/M_1-1/M$ to simplify this to

$$
\frac{\dot P_{\rm orb}}{P_{\rm orb}}
=-3f\frac{\dot M_1}{M_1}-3\frac{\dot M_2}{M_2}-2\frac{\dot M}{M}.
$$

For constant $f$, [integration](../../../../../integral.md) therefore gives

$$
\boxed{P_{\rm orb}\propto M_1^{-3f}M_2^{-3}(M_1+M_2)^{-2}.}
$$

This is the [donor-wind period invariant with fixed retention fraction](../../../../../donor-wind-period-invariant-with-fixed-retention-fraction.md). If $f$ changes during the evolution, the differential equation remains valid but the integrated invariant is instead $P_{\rm orb}M_2^3M^2\exp(3\int f\,d\log M_1)=\mathrm{constant}$. The fixed-power expression cannot be used with a time-dependent exponent without this modification.

For the [Roche lobe](../../../../../roche-lobe.md), write $q=M_1/M_2$. The equivalent separation expression $J=M_1M_2\sqrt{Ga/M}$ gives

$$
\frac{\dot a}{a}=2\frac{\dot J}{J}-2\frac{\dot M_1}{M_1}-2\frac{\dot M_2}{M_2}+\frac{\dot M}{M}
=\frac{\dot M_1}{M_1}\left[2f(q-1)-(1-f)\frac q{1+q}\right].
$$

Taking the [logarithmic derivative](../../../../../logarithmic-derivative.md) of $R_L=0.46a(M_1/M)^{1/3}$ then adds $\dot M_1/(3M_1)-\dot M/(3M)$, yielding

$$
\boxed{\frac{\dot R_L}{R_L}=\frac{\dot M_1}{M_1}\left[
f\left(2q+\frac{4q}{3(1+q)}-2\right)+\frac13-\frac{4q}{3(1+q)}\right].}
$$

This [donor-wind Roche-lobe response](../../../../../donor-wind-roche-lobe-response.md) uses only the instantaneous value of $f$ and thus still holds if it varies.

Define $A(q)=2q+4q/[3(1+q)]-2$ and $B(q)=1/3-4q/[3(1+q)]$. The [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md) is $\zeta_L=B+Af$, whereas the [donor star](../../../../../donor-star.md)'s [stellar radius response exponent](../../../../../stellar-radius-response-exponent.md) is $\zeta_*=-n$. Keeping $R_1=R_L$ requires the two [logarithmic derivatives](../../../../../logarithmic-derivative.md) of [radius](../../../../../radius.md) to agree, so

$$
\boxed{f\left(2q+\frac{4q}{3(1+q)}-2\right)=\frac{4q}{3(1+q)}-n-\frac13.}
$$

For $A\ne0$, this determines

$$
\boxed{f_{\rm req}=\frac{4q/[3(1+q)]-n-1/3}{2q+4q/[3(1+q)]-2}.}
$$

A physical mixture of [Roche-lobe overflow](../../../../../roche-lobe-overflow.md) and [stellar wind](../../../../../stellar-wind.md) from the [donor star](../../../../../donor-star.md) needs $0<f<1$. Equivalently, $-n$ must lie strictly between the pure-wind response $B$ and the conservative response $B+A=2q-5/3$. The values $f=0$ and $1$ are valid limiting prescriptions, respectively pure [stellar wind](../../../../../stellar-wind.md) and [conservative mass transfer](../../../../../conservative-binary-mass-transfer.md), rather than mixtures. If $f_{\rm req}$ lies outside $[0,1]$, no allowed division of the lost [mass](../../../../../mass.md) can maintain contact under this [radius](../../../../../radius.md) law and angular-momentum-loss prescription. This is [feasibility of donor-wind binary contact](../../../../../feasibility-of-donor-wind-binary-contact.md).

The likely direction away from contact follows without assigning a nonphysical fraction. For any actual $f$, let $\Delta=\log(R_1/R_L)$. Then

$$
\dot\Delta=(-n-B-Af)\frac{\dot M_1}{M_1}
=A(f_{\rm req}-f)\frac{\dot M_1}{M_1}.
$$

Since $\dot M_1<0$, a positive value of $A(f_{\rm req}-f)$ makes the [donor star](../../../../../donor-star.md) move inside its lobe and detach; a negative value increases overfill and promotes stronger transfer. Thus if $A>0$, $f_{\rm req}<0$ gives increasing overfill and $f_{\rm req}>1$ gives detachment; if $A<0$, these outcomes are reversed. A runaway or a new equilibrium would require the [donor star](../../../../../donor-star.md)'s response or the angular-momentum-loss model to change, possibly with additional driving. The contact calculation alone does not prove a particular nonlinear endpoint.

There is also a genuine exceptional denominator: $A=0$ at $q=(\sqrt{10}-1)/3$. At this ratio both limiting lobe responses coincide. Contact is possible only if $-n=B$, namely $n=(\sqrt{10}-2)/(\sqrt{10}+2)$; then every $f$ gives the same instantaneous [radius](../../../../../radius.md) response. Otherwise no fraction works, and the sign of $(-n-B)\dot M_1/M_1$ determines detachment or increasing overfill.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
