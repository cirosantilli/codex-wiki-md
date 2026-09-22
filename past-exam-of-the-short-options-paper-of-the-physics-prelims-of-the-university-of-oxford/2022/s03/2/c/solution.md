<h1 id="s03/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a normalized [quantum state](../../../../../quantum-state.md), $|\alpha|^2+|\beta|^2=1$, and the [Born rule](../../../../../born-rule.md) gives $\boxed{p(z+)=|\alpha|^2,\ p(z-)=|\beta|^2}$. If the displayed coefficients are not normalized, divide both by $|\alpha|^2+|\beta|^2$. A [quantum superposition](../../../../../quantum-superposition.md) is a coherent linear combination: relative phase affects other [spin](../../../../../spin.md) measurements, unlike an incoherent statistical mixture with the same $z$-measurement [probabilities](../../../../../probability.md).

Every pure [qubit](../../../../../qubit.md) [quantum state](../../../../../quantum-state.md) is an [eigenstate](../../../../../eigenstate.md) of [spin](../../../../../spin.md) along some axis. Its [Bloch vector](../../../../../bloch-vector.md) is

$$
\mathbf n=(2\operatorname{Re}(\alpha^*\beta),\ 2\operatorname{Im}(\alpha^*\beta),\ |\alpha|^2-|\beta|^2).
$$

For real normalized $\alpha,\beta$, choose $\theta$ modulo $2\pi$ with $\alpha=\cos(\theta/2)$ and $\beta=\sin(\theta/2)$, allowing an irrelevant global sign. Then

$$
\boxed{\mathbf n=(2\alpha\beta,0,\alpha^2-\beta^2),\qquad
S_{\mathbf n}|\psi\rangle=\frac{\hbar}{2}|\psi\rangle.}
$$

Equivalently, $S_{\mathbf n}=(\hbar/2)\begin{pmatrix}\alpha^2-\beta^2&2\alpha\beta\\2\alpha\beta&\beta^2-\alpha^2\end{pmatrix}$. A [Stern-Gerlach spin measurement](../../../../../stern-gerlach-spin-measurement.md) on this axis yields its positive result with certainty, so the state is not a nontrivial [quantum superposition](../../../../../quantum-superposition.md) in that measurement basis.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
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
