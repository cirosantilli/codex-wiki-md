<h1 id="23h/solution">Solution</h1>

↑ **Parent:** [23H](../23h.md)

The function $z\mapsto\wp(-z)$ has the same periodicity, poles and normalized Laurent behavior as $\wp(z)$. Uniqueness in its definition therefore makes $\wp$ even, so $\wp'$ is odd. At a nonzero half-period $b$ with $2b\in\Lambda$, periodicity and oddness give $\wp'(b)=\wp'(-b)=-\wp'(b)$, hence zero. Modulo $\Lambda$ the three such points are $1/2$, $\tau/2$, $(1+\tau)/2$.

An [elliptic function](../../../../../elliptic-function.md) has equal total orders of zeros and poles in a period cell, by the argument principle and cancellation of opposite boundary edges. The derivative has exactly one pole modulo the lattice, of order three at zero. The three displayed zeros therefore exhaust its zeros, each with multiplicity one:

$$
\boxed{\wp'(z)=0\iff z\equiv1/2,\tau/2,(1+\tau)/2\pmod\Lambda.}
$$

The only potential poles of $h$ outside the lattice are at $z=a$ and $z=-a$. Since $2a\notin\Lambda$, these points are distinct modulo the lattice and $\wp'(a)\ne0$. At each point the squared factor $(\wp(z)-\wp(a))^2$ vanishes to order two, canceling the double pole of the shifted [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md). The derivative term is regular there. Thus $h$ has no poles outside $\Lambda$.

Near zero write $\wp(z)=z^{-2}+c_2z^2+O(z^4)$, using evenness and the normalization. Taylor expansion at $a$ gives

$$
\wp(z-a)-\wp(z+a)=-2\wp'(a)z-\tfrac13\wp'''(a)z^3+O(z^5).
$$

Consequently

$$
h(z)=\left[4\wp(a)\wp'(a)-\tfrac13\wp'''(a)\right]z^{-1}+O(z).
$$

The $z^{-3}$ terms cancel exactly, and there are no $z^{-2}$ terms. Thus there is at most one simple pole per period cell. The sum of residues of an [elliptic function](../../../../../elliptic-function.md) over a period cell is zero, again because opposite boundary contour integrals cancel; its sole possible residue must vanish. Hence $h$ is entire. Periodicity makes it bounded on the plane, and [Liouville's theorem](../../../../../liouville-theorem.md) makes it constant. In fact $h$ is odd, so that constant is zero. The resulting [Weierstrass shift-difference identity by pole cancellation](../../../../../weierstrass-shift-difference-identity-by-pole-cancellation.md) is

$$
\boxed{h\equiv0.}
$$

## ↑ Ancestors (10)

1. [23H](../23h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
