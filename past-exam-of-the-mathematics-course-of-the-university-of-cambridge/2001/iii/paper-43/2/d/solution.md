<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the upward incident [internal gravity wave](../../../../../../internal-wave.md), $P=\rho_0\omega m_0W/k^2$. Using real physical fields, its time-averaged vertical [energy flux](../../../../../../energy-flux.md) per unit area is

$$
\mathcal I=\frac12\operatorname{Re}(PW^*)=\frac{\rho_0\omega m_0|w_0|^2}{2k^2}.
$$

The assumed mixing power is $\mathcal I/4$. A deepening law also requires the gravitational [potential energy](../../../../../../potential-energy.md) of the mixed layer. The wave problem specifies a well-mixed half-space above the interface, but supplies neither a finite upper mixed-layer depth nor a replacement buoyancy/energy boundary condition. There is therefore no unique finite-layer $d(t)$ from the printed information alone.

The missing parameter can be displayed explicitly. Let the initially mixed upper region have finite depth $a$, with a fixed upper boundary at $z=a$, and conserve its integrated [buoyancy](../../../../../../buoyancy.md) while homogenizing down to $z=-d$. Its new buoyancy is

$$
b_m=b_1-\frac{\Delta b\,d+N_0^2d^2/2}{a+d}.
$$

Integrate $-\rho_0zb$ over the initial and final profiles in $-d<z<a$. The [potential energy of mixed-layer deepening with an initial buoyancy jump](../../../../../../potential-energy-of-mixed-layer-deepening-with-an-initial-buoyancy-jump.md) is

$$
\frac{\Delta\mathcal P}{\rho_0}=\frac{\Delta b\,a d}{2}+\frac{N_0^2a d^2}{4}+\frac{N_0^2d^3}{12}.
$$

With $d(0)=0$ and a maintained constant incident flux, the resulting law is

$$
\boxed{\frac{\Delta b\,a d}{2}+\frac{N_0^2a d^2}{4}+\frac{N_0^2d^3}{12}
=\frac{\omega m_0|w_0|^2}{8k^2}t,\qquad
\dot d=\frac{\omega m_0|w_0|^2/(8k^2)}{\Delta b\,a/2+N_0^2a d/2+N_0^2d^2/4}.}
$$

The right-hand side is positive and determines a unique depth once $a$ is supplied. Initially $\dot d=\omega m_0|w_0|^2/(4k^2\Delta b\,a)$ for $a>0$, already showing why the upper depth matters. If the added assumptions instead specify a zero initial mixed depth, the cubic term gives $d=[3\omega m_0|w_0|^2t/(2k^2N_0^2)]^{1/3}$; the initial jump then has no finite volume above it to mix with. Neither assumption is contained in the original half-space wave statement. Literal homogenization of the entire upper half-space is the $a\to\infty$ limit and costs infinite energy for any fixed positive $d$. This limitation should not be concealed by a guessed entrainment depth or by keeping the upper buoyancy fixed while claiming conservation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
