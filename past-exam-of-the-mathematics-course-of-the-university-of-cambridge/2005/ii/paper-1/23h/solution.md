<h1 id="23h/solution">Solution</h1>

↑ **Parent:** [23H](../23h.md)

The local estimate gives $\wp(z)=z^{-2}+O(z)$ at zero and, by periodicity, at every lattice point. If two candidates existed, their difference would extend to an entire doubly periodic function: the principal parts cancel at every possible pole. It is bounded on a fundamental parallelogram, hence on the plane, so [Liouville theorem](../../../../../liouville-theorem.md) makes it constant. The local $O(z)$ difference tends to zero, making the constant zero. Thus **the function is unique**.

The function $z\mapsto\wp(-z)$ has the same periodicity, poles and local estimate. Uniqueness therefore proves **$\wp(-z)=\wp(z)$**. Its Laurent expansion is consequently

$$
\wp(z)=z^{-2}+c_2z^2+c_4z^4+\cdots,
$$

with no constant term by the given estimate. Periodicity and evenness imply $\wp(1/2+t)=\wp(1/2-t)$, so $\wp'(1/2)=0$. The elliptic zero-pole counting theorem says a nonconstant [elliptic function](../../../../../elliptic-function.md) has, in one period cell, equally many zeros and poles counted with multiplicity. Applied to $\wp(z)-\wp(1/2)$, whose total pole order is two, it gives precisely two zeros counted with multiplicity. The zero at $1/2$ already has multiplicity at least two. It therefore has exactly two, proving

$$
\boxed{\wp''(1/2)\ne0.}
$$

Finally $\wp''-6\wp^2$ is periodic, and the Laurent expansion shows cancellation of all possible pole terms: $\wp''=6z^{-4}+2c_2+O(z^2)$ and $6\wp^2=6z^{-4}+12c_2+O(z^2)$. The difference extends to an entire bounded function and is constant. Hence

$$
\boxed{\wp''(z)=6\wp(z)^2+A,\qquad A=-10c_2.}
$$

Every property of the [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) used here has been obtained from the stated local and periodic properties, together with the explicitly stated standard elliptic-function counting theorem.

## ↑ Ancestors (10)

1. [23H](../23h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
