# Factorization through a surjection

↑ **Parent:** [Fiber of a function](fiber-of-a-function.md)

For a [surjective function](surjective-function.md) $f:B\to A$ and a function $g:B\to C$, there is a unique function $h:A\to C$ with $g=h\circ f$ if and only if $g$ is constant on each [fiber of a function](fiber-of-a-function.md) of $f$. Define $h(a)$ to be the common value on $f^{-1}(a)$; it is well-defined and unique because that fiber is nonempty. This uniquely specified value requires no simultaneous arbitrary choices.

For a concrete example, restrict the [codomain](codomain.md) of the finite [function](function-split.md) above to its [image of a function](image-of-a-function.md) $I=\{0,1,2\}$, making $f:A\to I$ [surjective](surjective-function.md). Define $g(a)=g(b)=5$, $g(c)=7$ and $g(d)=9$. Then $h(y)=2y+5$ on $I$ gives $g=h\circ f$: knowing the output of $f$ is enough to compute $g$. If instead $g(a)\ne g(b)$, no such $h$ can exist, because $h(f(a))=h(f(b))$ must be the same value.

The [surjectivity](surjective-function.md) assumption supplies uniqueness on the full target. If the original unused target value three were retained, the factorization would impose no condition on $h(3)$, and different extensions could agree on every actual input. Thus [factorization through a surjection](factorization-through-a-surjection.md) formalizes when a compressed description retains all information needed for a later calculation.

// Target: combinatorics.bigb

## ↑ Ancestors (7)

1. [Fiber of a function](fiber-of-a-function.md)
2. [Function](function-split.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Factorization through a surjection](factorization-through-a-surjection.md)
- [Fiber of a function](fiber-of-a-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-4/5e/b/solution.md)
