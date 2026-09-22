<h1 id="16c/solution">Solution</h1>

↑ **Parent:** [16C](../16c.md)

In a source-free vacuum, [Maxwell equations](../../../../../maxwell-equations.md) are

$$
\nabla\cdot\mathbf E=0,\quad\nabla\cdot\mathbf B=0,\quad\nabla\times\mathbf E=-\partial_t\mathbf B,\quad\nabla\times\mathbf B=\mu_0\epsilon_0\partial_t\mathbf E.
$$

Taking a [curl](../../../../../curl.md) of the last two equations and using $\nabla\times(\nabla\times\mathbf A)=\nabla(\nabla\cdot\mathbf A)-\nabla^2\mathbf A$ gives the [electromagnetic wave equations](../../../../../electromagnetic-wave-equation.md)

$$
\boxed{\mathbf E_{tt}=c^2\nabla^2\mathbf E,\quad\mathbf B_{tt}=c^2\nabla^2\mathbf B,\quad c=\frac1{\sqrt{\mu_0\epsilon_0}}}.
$$

Substitution of the complex [plane wave](../../../../../plane-wave.md) amplitudes into [Maxwell equations](../../../../../maxwell-equations.md), then taking real parts, gives

$$
\mathbf k\cdot\mathbf e=\mathbf k\cdot\mathbf b=0,\qquad\mathbf k\times\mathbf e=\omega\mathbf b,\qquad\mathbf k\times\mathbf b=-\frac\omega{c^2}\mathbf e.
$$

For a nonzero propagating wave these imply the [dispersion relation](../../../../../dispersion-relation.md) $\boxed{\omega^2=c^2|\mathbf k|^2}$. Conversely choose any nonzero transverse complex $\mathbf e$ and set $\mathbf b=\mathbf k\times\mathbf e/\omega$ to obtain such a wave. The static uniform-field sector at $\omega=|\mathbf k|=0$ is separate from propagation.

At a [perfect conductor](../../../../../perfect-conductor.md), the oscillatory boundary conditions are $\mathbf n\times\mathbf E=0$ and $\mathbf n\cdot\mathbf B=0$. Surface charge and surface current allow nonzero normal electric and tangential magnetic fields. The magnetic condition here concerns the time-dependent wave field; a perfect conductor can retain a pre-existing static magnetic field.

Let $R=I-2\mathbf n\mathbf n^T$ be the orthogonal reflection across the boundary plane, so $\det R=-1$. The proposed reflected amplitudes are $\mathbf k'=R\mathbf k$, $\mathbf e'=-R\mathbf e$, and $\mathbf b'=R\mathbf b$. For an orthogonal reflection, $(R\mathbf a)\times(R\mathbf d)=-R(\mathbf a\times\mathbf d)$. Hence

$$
\mathbf k'\times\mathbf e'=\omega\mathbf b',\qquad\mathbf k'\times\mathbf b'=-\frac\omega{c^2}\mathbf e',\qquad\mathbf k'\cdot\mathbf e'=\mathbf k'\cdot\mathbf b'=0.
$$

Also $|\mathbf k'|=|\mathbf k|$, so the reflected wave obeys the same [dispersion relation](../../../../../dispersion-relation.md). At $\mathbf n\cdot\mathbf x=0$, the incident and reflected phases coincide because $\mathbf k'-\mathbf k$ is parallel to $\mathbf n$. Their summed amplitudes satisfy

$$
\mathbf e+\mathbf e'=2(\mathbf n\cdot\mathbf e)\mathbf n,\qquad\mathbf b+\mathbf b'=2[\mathbf b-(\mathbf n\cdot\mathbf b)\mathbf n].
$$

The first has zero tangential part and the second zero normal part, proving both boundary conditions. Finally $\mathbf k'\cdot\mathbf n=-\mathbf k\cdot\mathbf n>0$, as required for reflection into the vacuum.

## ↑ Ancestors (10)

1. [16C](../16c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
