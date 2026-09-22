<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

For the sum $F=f+g$:

- In case (a), **yes**. If $F$ were [differentiable](../../../../../differentiable-function.md) at $a$, then $g=F-f$ would be differentiable there, contrary to the hypothesis.
- In case (b), **no**. Take$$
  f(x)=|x-a|,\qquad g(x)=-|x-a|.
  $$

  Both are continuous and nondifferentiable at $a$, but $F=0$ is differentiable.

For the product $G=fg$, the answer is **no** in both cases:

- For case (a), take $f(x)=x-a$ and $g(x)=|x-a|$. Then $f$ is differentiable at $a$, $g$ is not, but$$
  G(x)=(x-a)|x-a|
  $$

  has derivative $0$ at $a$.
- For case (b), take $f(x)=g(x)=|x-a|$. Neither factor is differentiable at $a$, whereas$$
  G(x)=(x-a)^2
  $$

  is differentiable.

Every displayed $f$ and $g$ is a [continuous function](../../../../../continuous-function.md) and is nonzero at points arbitrarily close to $a$, so the extra condition in the question is satisfied.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
