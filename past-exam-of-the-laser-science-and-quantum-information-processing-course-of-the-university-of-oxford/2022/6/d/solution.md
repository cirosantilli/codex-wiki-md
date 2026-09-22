<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Encode $0$ by phase zero and $1$ by phase $\pi$. Alice and Bob choose their bits independently and keep their choices private. Bob announces the trial numbers with a D0 click over an authenticated public channel. For each retained trial, [c](../c.md) guarantees that their bits agree. In the ideal symmetric setup, the two equal-phase cases $00$ and $11$ give the same click probability, so announcing success does not itself reveal which shared bit was used.

The matching-phase cases occur with [probability](../../../../probability.md) $1/2$, and a matching case succeeds with [probability](../../../../probability.md) $1/16$. Therefore

$$
\boxed{P(\text{retained trial})=\frac1{32},\qquad
\mathbb E[K_{\rm raw}]=\frac N{32}.}
$$

For independent ideal trials, the raw-key length has a [binomial distribution](../../../../binomial-distribution.md) with [standard deviation](../../../../standard-deviation.md) $\sqrt{31N}/32$. These are bits before sacrificing test positions or performing [privacy amplification](../../../../privacy-amplification.md).

A missing click does **not** certify unequal phases: the same phases also fail to click with [probability](../../../../probability.md) $15/16$. With uniform choices,

$$
P(\phi_A=\phi_B\mid\text{no click})=\frac{15}{31},\qquad
P(\phi_A\ne\phi_B\mid\text{no click})=\frac{16}{31}.
$$

Thus a no-click trial supplies neither a known equal bit nor a known complemented bit. This is why it cannot be retained by the direct error-free sifting rule. The source's “cannot use” should be understood in this sense: the events are not statistically independent, so an absolute claim that they contain no information would be false.

To obtain a secret final key, reveal and discard a random subset of retained bits to test the observed error rate, then apply reconciliation and [privacy amplification](../../../../privacy-amplification.md) as required by a security analysis of the actual implementation. Resolving which time path a [photon](../../../../photon.md) took removes the accepted histories' [quantum coherence](../../../../quantum-coherence-in-a-specified-basis.md) and can turn destructive [interference](../../../../interference-wave-propagation.md) into false D0 clicks, providing a simple disturbance test. Equal-phase click correlations alone are not a proof of security against every attack, particularly in the presence of losses and device imperfections. The supplied ideal model fixes the sifted rate $N/32$; it does not fix a positive secure final length without an adversary model and observed parameters.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
