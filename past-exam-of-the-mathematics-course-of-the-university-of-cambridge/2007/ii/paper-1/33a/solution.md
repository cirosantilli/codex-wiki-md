<h1 id="33a/solution">Solution</h1>

↑ **Parent:** [33A](../33a.md)

The incoming and outgoing coefficients give the [scattering matrix](../../../../../s-matrix.md)

$$
\boxed{S(k)=\frac{g(k)}{g(-k)}=\frac{(k+i\kappa)(k+i\alpha)}{(k-i\kappa)(k-i\alpha)}.}
$$

It obeys $S(-k)=S(k)^{-1}$ and $S(k^*)^*=S(k)^{-1}$, so $|S(k)|=1$ for real $k$, as required by elastic [unitarity](../../../../../unitary-operator.md). With $S=e^{2i\delta}$, the [scattering phase shift](../../../../../scattering-phase-shift.md) satisfies $\tan\delta=k(\kappa+\alpha)/(k^2-\kappa\alpha)$. The inverse tangent needs a continuous branch: taking $\delta(\infty)=0$ gives $\delta(0)=\pi$. Equivalently $\delta=\arctan(\kappa/k)+\arctan(\alpha/k)$ for $k>0$.

The [scattering length](../../../../../scattering-length-from-a-partial-wave-s-matrix.md) follows from $k\cot\delta=-1/a_s+O(k^2)$:

$$
\boxed{a_s=\frac{\kappa+\alpha}{\kappa\alpha}.}
$$

For a putative bound state put $k=i\eta$, $\eta>0$. The incoming term grows as $e^{\eta r}$, so its coefficient must vanish. The incoming [Jost function](../../../../../jost-function.md) is $F(k)=g(-k)=(k-i\kappa)/(k+i\alpha)$; its only upper-half-plane zero is $i\kappa$. Under the regular-potential assumption this gives **one bound state**, with $\boxed{E=-\hbar^2\kappa^2/(2m).}$ The pole at $i\alpha$ in $S$ instead comes from the outgoing numerator: it is a [redundant pole of a scattering matrix](../../../../../redundant-pole-of-a-scattering-matrix.md), not a second normalizable state. The S-matrix alone, without its incoming/outgoing analytic structure, would tempt an incorrect count of two states.

For completeness, the nonsingular Eckart realization of this Jost function requires $\alpha>\kappa$, as discussed in [https://dipot.ulb.ac.be/dspace/bitstream/2013/373712/4/2306.12216.pdf.](https://dipot.ulb.ac.be/dspace/bitstream/2013/373712/4/2306.12216.pdf.) The supplied positive constants alone do not establish such a realization in every ordering; a coincident pole is likewise not evidence for two states.

There is no positive-energy [scattering resonance](../../../../../scattering-resonance.md). Indeed $\delta'(k)=-\kappa/(k^2+\kappa^2)-\alpha/(k^2+\alpha^2)<0$, and the s-wave total [partial-wave total scattering cross-section](../../../../../partial-wave-total-scattering-cross-section.md) is $4\pi(\kappa+\alpha)^2/[(k^2+\kappa^2)(k^2+\alpha^2)]$, strictly decreasing for $k>0$. All poles are on the imaginary axis, with no oscillatory decaying resonance pole.

## ↑ Ancestors (10)

1. [33A](../33a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
