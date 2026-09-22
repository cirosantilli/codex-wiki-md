<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

[Path tracing](../../../../../path-tracing.md) estimates the [rendering equation](../../../../../rendering-equation.md) by a [Monte Carlo method](../../../../../monte-carlo-method-split.md). Launch camera [rays](../../../../../ray-geometry.md); at each surface hit sample an outgoing continuation direction according to a chosen [probability density function](../../../../../probability-density-function.md), trace to the next hit, and continue through successive reflections. Accumulate emitted light or environment light with the product of scattering, cosine and inverse-density factors along the path. A bounce sampled with density $p(\omega)$ updates the path weight by

$$
\boxed{\beta\leftarrow\beta\,\frac{f_r(\omega,\omega_o)|\hat N\cdot\omega|}{p(\omega)}.}
$$

Average many independently sampled paths per [pixel](../../../../../pixel.md). Multiple bounces account for indirect illumination, including colour bleeding between surfaces, instead of approximating all of it by one ambient constant. Termination can use [Russian roulette](../../../../../russian-roulette-monte-carlo.md): continue with probability $q>0$ and divide surviving weights by $q$, preserving the expected contribution. A fixed bounce cutoff is simpler but truncates transport.

The elementary strategy that obtains illumination only when a randomly continued path _hits an emitter_ fails for ideal point lights. From a surface [point](../../../../../point-geometry.md), an ideal point source occupies zero [solid angle](../../../../../solid-angle.md); sampling a direction from an ordinary continuous [probability density function](../../../../../probability-density-function.md) hits that one direction with probability zero. Thus this strategy almost surely never discovers the light, regardless of the number of samples. An area emitter occupies nonzero [solid angle](../../../../../solid-angle.md) and can be hit.

The qualification matters: practical [path tracing](../../../../../path-tracing.md) can use point lights by explicitly sampling a source and connecting the current surface to it with a [shadow ray](../../../../../shadow-ray.md), a technique called [next-event estimation](../../../../../next-event-estimation.md). For a point source the connection direction is known exactly, rather than discovered by a random hemisphere hit. Thus the restriction applies to naive emitter-hit [path tracing](../../../../../path-tracing.md), not to all [path tracing](../../../../../path-tracing.md) algorithms.[§12.2: point lights have delta-position emission and deterministic incident directions; §13.4: direct-light sampling is combined with scattering-direction sampling](../../../../../physically-based-rendering-from-theory-to-implementation-4th-edition-by-matt-pharr-and-others.md)

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Computer graphics](../../../computer-graphics-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
