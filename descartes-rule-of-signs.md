# Descartes' rule of signs

↑ **Parent:** [Polynomial](polynomial-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Descartes'_rule_of_signs)

Let $V(p)$ be the number of sign changes in the list of nonzero coefficients of a real [polynomial](polynomial-split.md), arranged by increasing or decreasing degree. The [positive roots of a polynomial](positive-root-of-a-polynomial.md), counted with [multiplicity of a root](multiplicity-of-a-root.md), satisfy

$$
N_+(p)\le V(p),\qquad V(p)-N_+(p)\text{ is even}.
$$

The bound follows by induction on the nonzero terms after removing the lowest power of $x$. Differentiation removes the constant coefficient. If it and the next coefficient have opposite signs, the [Rolle root count with multiplicities](rolle-root-count-with-multiplicities.md) loses at most one root and the sign-change count loses one. If their signs agree, the derivative must have an extra root before the first positive root, so neither count needs that extra allowance. The parity statement follows by comparing the signs near zero and at positive infinity: roots of odd multiplicity reverse the sign, and roots of even multiplicity preserve it. Apply the same rule to $p(-x)$ to bound negative roots.

## ↑ Ancestors (5)

1. [Polynomial](polynomial-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/10e/solution.md)
