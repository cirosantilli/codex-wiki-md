<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathbf u_\theta=(\cos\theta,\sin\theta)^{\mathsf T}$ be the transmission direction. An ideal linear [polarizer](../../../../../polarizer.md) projects the incident [electric field](../../../../../electric-field-split.md) onto this direction, so its [Jones matrix](../../../../../jones-matrix.md) is

$$
\boxed{P(\theta)=\mathbf u_\theta\mathbf u_\theta^{\mathsf T}
=\begin{pmatrix}\cos^2\theta&\cos\theta\sin\theta\\
\cos\theta\sin\theta&\sin^2\theta\end{pmatrix}}.
$$

Since $\mathbf u_\beta^{\mathsf T}\mathbf u_\alpha=\cos(\alpha-\beta)$, the [amplitude](../../../../../wave-amplitude.md) transmitted by a sequence of [polarizers](../../../../../polarizer.md) is the product of the projections between successive axes. Here the four directions are $0,\omega t,-2\omega t,0$. After the first [polarizer](../../../../../polarizer.md) the [unpolarized light](../../../../../unpolarized-light.md) input has intensity $I/2$ and is in [linear polarization](../../../../../linear-polarization.md) along $x$. The [transmission through a sequence of linear polarizers](../../../../../transmission-through-a-sequence-of-linear-polarizers.md) therefore follows from successive applications of [Malus's law](../../../../../malus-s-law.md)

$$
\boxed{I_{\rm out}(t)=\frac I2\cos^2(\omega t)\cos^2(3\omega t)\cos^2(2\omega t)}.
$$

The relative angle between the rotating [polarizers](../../../../../polarizer.md) is $3\omega t$, not $\omega t$. The first factor $1/2$ is an [ensemble average](../../../../../expected-value-split.md) over incident polarization: [unpolarized light](../../../../../unpolarized-light.md) cannot be represented by a single deterministic [Jones vector](../../../../../jones-vector.md). Equivalently, its [coherency matrix](../../../../../coherency-matrix.md) is $(I/2)I_2$; the total [matrix](../../../../../matrix.md) $P(0)P(-2\omega t)P(\omega t)P(0)$ gives the same output intensity by the [trace](../../../../../matrix-trace.md) rule. The quasistatic optical-element approximation assumes the mechanical rotation is slow compared with the optical oscillation.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
