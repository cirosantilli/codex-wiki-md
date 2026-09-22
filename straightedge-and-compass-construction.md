# Straightedge and compass construction

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Straightedge_and_compass_construction)

A [compass-and-straightedge construction](straightedge-and-compass-construction.md) uses an unmarked straightedge to draw a [Euclidean line](euclidean-geometry.md#straight-line) through two already constructed points, and a compass to draw a [circle](topology.md#circle) with a constructed centre and radius. New points arise from intersections of these lines and circles. The allowed operations matter: an accurate numerical drawing need not supply such a construction.

**Table of contents**

- [General angle quintisection is impossible with straightedge and compass](#general-angle-quintisection-is-impossible-with-straightedge-and-compass)
- [Impossibility of doubling the cube by straightedge and compass](#impossibility-of-doubling-the-cube-by-straightedge-and-compass)
- [Constructible polygon](#constructible-polygon)
  - [Constructible regular polygon](#constructible-regular-polygon)
    - [Gauss-Wantzel theorem](#gauss-wantzel-theorem)

## General angle quintisection is impossible with straightedge and compass

↑ **Parent:** [Straightedge and compass construction](straightedge-and-compass-construction.md)

Consider the constructible angle whose cosine is $5/6$ and sine is $\sqrt{11}/6$. If one fifth of this angle were constructible, its cosine $c$ would satisfy the displayed polynomial, by the identity $\cos5\theta=16\cos^5\theta-20\cos^3\theta+5\cos\theta$. The identity follows by taking the real part of $(\cos\theta+i\sin\theta)^5$ and substituting $\sin^2\theta=1-\cos^2\theta$.

The polynomial is irreducible by [Eisenstein's criterion](commutative-algebra.md#eisenstein-criterion) at five, so $c$ has degree five over the rational numbers. The initial angle field $\mathbb Q(\sqrt{11})$ already has degree two, and adjoining any finite collection of [constructible numbers](galois-theory.md#constructible-number) gives total degree over the rational numbers a power of two. Such a field cannot contain the degree-five element $c$, by the [tower law for field extensions](galois-theory.md#tower-law-for-field-extensions). Hence this constructible angle cannot be divided into five equal angles by [straightedge and compass construction](straightedge-and-compass-construction.md). Some particular angles can be quintisected; the obstruction disproves a construction valid for all angles.

## Impossibility of doubling the cube by straightedge and compass

↑ **Parent:** [Straightedge and compass construction](straightedge-and-compass-construction.md)

Doubling the volume of a unit cube requires constructing its new side length $\sqrt[3]2$. Its minimal polynomial $X^3-2$ is irreducible by [Eisenstein's criterion](commutative-algebra.md#eisenstein-criterion) at two, so this length has degree three. Every [constructible number](galois-theory.md#constructible-number) belongs to a finite tower of quadratic extensions, whose total degree is a power of two. The [tower law for field extensions](galois-theory.md#tower-law-for-field-extensions) would force the degree three to divide that power of two, a contradiction. Thus no such [straightedge and compass construction](straightedge-and-compass-construction.md) exists.

## Constructible polygon

↑ **Parent:** [Straightedge and compass construction](straightedge-and-compass-construction.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constructible_polygon)

A [constructible polygon](#constructible-polygon) is a [polygon](euclidean-geometry.md#polygon) whose vertices can be obtained by a [compass-and-straightedge construction](straightedge-and-compass-construction.md) from the specified initial data. The classical question for a [regular polygon](euclidean-geometry.md#regular-polygon) asks which numbers of sides permit an exact construction from a given side or circumscribed [circle](topology.md#circle).

### Constructible regular polygon

↑ **Parent:** [Constructible polygon](#constructible-polygon)

A [constructible regular polygon](#constructible-regular-polygon) is a [regular polygon](euclidean-geometry.md#regular-polygon) admitting a [compass-and-straightedge construction](straightedge-and-compass-construction.md). The [Gauss-Wantzel theorem](#gauss-wantzel-theorem) classifies its possible numbers of sides.

#### Gauss-Wantzel theorem

↑ **Parent:** [Constructible regular polygon](#constructible-regular-polygon)

For $N\geq3$, a [regular polygon](euclidean-geometry.md#regular-polygon) with $N$ sides is a [constructible regular polygon](#constructible-regular-polygon) exactly when $N=2^a p_1\cdots p_r$, where $a$ is a [nonnegative integer](arithmetic.md#natural-number) and the $p_j$ are distinct [Fermat primes](prime-number.md#fermat-prime); the product may be empty. Thus seventeen and fifteen qualify, while nine does not. [Carl Friedrich Gauss](mathematics.md#carl-friedrich-gauss) established sufficiency, and [Pierre Wantzel](mathematics.md#pierre-wantzel) proved necessity in 1837.[slide 18](mathematics-bibliography.md#primality-testing-then-and-now-by-carl-pomerance)

## ↑ Ancestors (5)

1. [Euclidean geometry](euclidean-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (7)

- [General angle quintisection is impossible with straightedge and compass](#general-angle-quintisection-is-impossible-with-straightedge-and-compass)
- [Impossibility of doubling the cube by straightedge and compass](#impossibility-of-doubling-the-cube-by-straightedge-and-compass)
- [Solution](past-exam-of-the-number-theory-course-of-the-university-of-oxford/2007.md#a/4/solution)
- [Solution](past-exam-of-the-number-theory-course-of-the-university-of-oxford/2008.md#a/4/solution)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2013.md#a/1/c/solution)
- [Solution](past-exam-of-the-options-i-for-mathematics-and-philosophy-course-of-the-university-of-oxford/2013.md#a/1/c/solution)
- [Regular heptagon](euclidean-geometry.md#regular-heptagon)
