<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Quantum error correction](../../../../quantum-error-correction-split.md) detects an error syndrome and actively restores a logical state within a correctable error set. A [decoherence-free subspace](../../../../decoherence-free-subspace.md) instead encodes into a subspace on which every allowed noise operator acts as the same scalar; no relative logical phase or mixing is produced by that noise. It relies on the specified correlation structure, and does not protect against arbitrary independent errors.

For collective rotations $R_z(\phi)\otimes R_z(\phi)$,

$$
|01\rangle\mapsto e^{-i\phi/2}e^{i\phi/2}|01\rangle=|01\rangle,
\qquad |10\rangle\mapsto|10\rangle.
$$

Thus every encoded superposition $\alpha|01\rangle+\beta|10\rangle$ is invariant. Equivalently it lies in the zero-eigenvalue subspace of $Z\otimes I+I\otimes Z$.

By contrast,

$$
\alpha|00\rangle+\beta|11\rangle
\mapsto\alpha e^{-i\phi}|00\rangle+\beta e^{i\phi}|11\rangle.
$$

The relative phase changes by $2\phi$, although $Z\otimes Z$ acts as $+I$ on both basis states. Invariance under one discrete operation does not establish invariance under its continuous rotation family. A concrete counterexample is $\phi=\pi/2$: the equally weighted encoded plus state becomes the encoded minus state, up to a global phase, and is orthogonal to its original state.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
