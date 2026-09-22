<h1 id="11i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume (i), and suppose a map $f$ as in (ii) existed. Then

$$
A=f^{-1}(I),\qquad B=f^{-1}(J),\qquad C=f^{-1}(K)
$$

are closed, cover $T$, and contain $I,J,K$, respectively. But

$$
A\cap B\cap C=f^{-1}(I\cap J\cap K)=\varnothing,
$$

since the three sides have no common point. This contradicts (i), so (i) implies (ii).

Conversely, suppose (i) fails. Let $A,B,C$ be a counterexample and put

$$
d_A(x)=\operatorname{dist}(x,A),\quad
d_B(x)=\operatorname{dist}(x,B),\quad
d_C(x)=\operatorname{dist}(x,C).
$$

No point lies in all three closed sets, so $D=d_A+d_B+d_C>0$. Identify $T$ affinely with the standard simplex so that side $I$ is the side on which the first barycentric coordinate is zero, and similarly for $J,K$. Define $f(x)$ to be the point with barycentric coordinates

$$
\frac1D(d_A(x),d_B(x),d_C(x)).
$$

Because $A\cup B\cup C$ covers $T$, at least one distance is zero, so $f(x)\in\partial T$. If $x\in I\subset A$, then $d_A(x)=0$, so $f(x)\in I$; likewise for $J,K$. Thus $f$ is a forbidden map from (ii). This proves (ii) implies (i).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11I](../../11i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
