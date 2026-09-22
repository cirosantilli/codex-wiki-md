<h1 id="7b/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the complex similarity [matrix](../../../../../../matrix.md) as

$$
S=X+iY,
$$

with $X,Y$ real. From $C=SDS^{-1}$ we obtain $CS=SD$, and equating real and imaginary parts gives

$$
CX=XD,\qquad CY=YD.
$$

Therefore

$$
C(X+tY)=(X+tY)D
$$

for every real $t$.

Now $p(t)=\det(X+tY)$ is a real [polynomial](../../../../../../polynomial-split.md) and

$$
p(i)=\det(X+iY)=\det S\ne0.
$$

Thus some real $t$ has $p(t)\ne0$. Taking $T=X+tY$, we have a real invertible [matrix](../../../../../../matrix.md) satisfying $CT=TD$, or

$$
\boxed{C=TDT^{-1}}.
$$

This proves [real similarity from complex similarity](../../../../../../real-similarity-from-complex-similarity.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
