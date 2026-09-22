<h1 id="24f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A derivation of $A$ centred at the $k$-point $p:A\to k$ is a $k$-linear map $D:A\to k$ satisfying the twisted [Leibniz rule](../../../../../../leibniz-rule.md)

$$
D(ab)=p(a)D(b)+p(b)D(a).
$$

The [Zariski tangent space](../../../../../../zariski-tangent-space.md) is

$$
T_pA=\operatorname{Der}(A,p).
$$

Since $p(f)\ne0$, $p$ extends uniquely to the [localization](../../../../../../localization-of-a-ring.md) $A[f^{-1}]$ by $p(a/f^n)=p(a)/p(f)^n$. Restriction gives a linear map

$$
T_pA[f^{-1}]\longrightarrow T_pA.
$$

Conversely, every $D\in T_pA$ has the unique extension

$$
\widetilde D\!\left(\frac a{f^n}\right)
=\frac{D(a)}{p(f)^n}
-\frac{n\,p(a)D(f)}{p(f)^{n+1}}.
$$

The quotient rule verifies the Leibniz identity, and the assumption that $f$ is not a zero divisor makes the localization representation compatible with equality of fractions. Extension and restriction are inverse, so the natural map is an isomorphism.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [24F](../../24f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
