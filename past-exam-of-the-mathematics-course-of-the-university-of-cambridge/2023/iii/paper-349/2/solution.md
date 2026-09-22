<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Direct evidence for [stellar feedback](../../../../../stellar-feedback.md) includes expanding ionized shells and superbubbles around young associations, hot X-ray-emitting gas in [supernova remnants](../../../../../supernova-remnant.md), broad or split emission lines, and blueshifted absorption showing cool and warm [outflows](../../../../../galactic-outflow.md). P-Cygni profiles reveal massive-star winds, while extraplanar filaments and metal-enriched gas demonstrate transport away from star-forming disks. Indirect evidence includes the galaxy mass--metallicity relation, low baryon fractions and suppressed star formation in dwarf galaxies, chemically enriched circumgalactic gas, and correlations of outflow speed and mass loading with the [star formation rate](../../../../../star-formation-rate.md).

Rapid gas removal changes the gravitational potential before stellar and dark-matter orbits can respond adiabatically. Positions and velocities are initially unchanged, but orbital binding energies rise; orbits expand and become more eccentric, and some particles escape. Repeated burst--outflow--reaccretion cycles can irreversibly transfer energy to collisionless matter and turn a central dark-matter cusp into a core. This matters because dwarf-galaxy rotation curves are used to test dark-matter microphysics: a feedback-made core can mimic a non-cold or self-interacting dark-matter signature.

Write the initial potential energy as $W=-aGM^2/R$. The [virial theorem](../../../../../virial-theorem.md) gives $T=-W/2$. If a well-mixed fraction $\epsilon$ remains after instantaneous mass loss, the immediate kinetic and potential energies are $T_a=\epsilon T$ and $W_a=\epsilon^2W$, so

$$
E_a=T_a+W_a
=a\frac{GM^2}{R}\left(\frac\epsilon2-\epsilon^2\right).
$$

After revirialization at $R'$, $E_f=W_f/2=-aG\epsilon^2M^2/(2R')$. Equating energies gives the [impulsive mass-loss expansion law](../../../../../impulsive-mass-loss-expansion-law.md)

$$
\boxed{\frac{R'}R=\frac{\epsilon}{2\epsilon-1}.}
$$

The remnant is bound only for $\epsilon>1/2$; loss of half or more of the gravitating mass disrupts this idealized system.

For many infinitesimal, individually revirialized losses, put $\epsilon=1+dM/M$ in the impulsive result. To first order, $dR/R=-dM/M$. Integration yields the [adiabatic mass-loss expansion law](../../../../../adiabatic-mass-loss-expansion-law.md)

$$
\boxed{MR=\text{constant},\qquad \frac{R'}R=\frac1\epsilon.}
$$

Slow loss causes finite expansion for every positive remaining mass fraction and has no sharp disruption threshold.

Finally consider an initially circular orbit of radius $R$ around a point mass $M$. Its speed and specific angular momentum obey $v^2=GM/R$ and $h^2=GMR$. Immediately after $M\to\epsilon M$, these remain unchanged, while the new specific energy is

$$
E'=\frac{GM}{R}\left(\frac12-\epsilon\right).
$$

Using the [orbital eccentricity](../../../../../orbital-eccentricity.md) relation $e^2=1+2E'h^2/(G^2\epsilon^2M^2)$ gives

$$
\boxed{e=\frac{1-\epsilon}{\epsilon}.}
$$

It is an ellipse for $\epsilon>1/2$, parabolic at $\epsilon=1/2$, and unbound for smaller $\epsilon$, in agreement with the virial argument.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
