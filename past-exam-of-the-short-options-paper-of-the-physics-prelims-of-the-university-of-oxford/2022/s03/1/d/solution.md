<h1 id="s03/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a monochromatic [photon](../../../../../photon.md) of vacuum [wavelength](../../../../../wavelength.md) $\lambda$, a plate of thickness $d$ replaces air by glass and adds phase $\phi=2\pi(n-1)d/\lambda$. Neglect losses and reflections, or assume antireflection coatings. Between the first [beam splitter](../../../../../beam-splitter.md) and mirror 1, the affected arm is the second basis component, so $D_\phi=\operatorname{diag}(1,e^{i\phi})$. The successive [quantum states](../../../../../quantum-state.md), omitting common propagation phases, are

$$
\begin{aligned}
\binom10&\xrightarrow{B}\frac1{\sqrt2}\binom11
\xrightarrow{D_\phi}\frac1{\sqrt2}\binom1{e^{i\phi}}
\xrightarrow{M}-\frac1{\sqrt2}\binom{e^{i\phi}}1\\
&\xrightarrow{B}-\frac12\binom{e^{i\phi}-1}{e^{i\phi}+1}.
\end{aligned}
$$

The first output component feeds detector 2 and the second feeds detector 1, giving

$$
\boxed{p_2=\sin^2(\phi/2),\qquad p_1=\cos^2(\phi/2).}
$$

The imbalance gives $p_1-p_2=\cos\phi$. Thus the measured [probabilities](../../../../../probability.md) determine only $\phi$ up to $\phi\mapsto\pm\phi+2\pi m$, and hence only a corresponding family of thicknesses. There is no unique absolute thickness from this one measurement. The zero-plate limit recovers $p_1=1$, $p_2=0$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [S03](../../../s03.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
