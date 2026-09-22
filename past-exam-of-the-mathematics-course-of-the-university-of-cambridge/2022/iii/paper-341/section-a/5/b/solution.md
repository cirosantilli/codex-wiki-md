<h1 id="section-a/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [Strang splitting](../../../../../../../strang-splitting.md)

$$
F(t)=e^{tA/2}e^{tB}e^{tA/2},
$$

reversing $t$ reverses all three factors, so

$$
F(-t)=e^{-tA/2}e^{-tB}e^{-tA/2}=F(t)^{-1}.
$$

It is therefore a [time-symmetric numerical method](../../../../../../../time-symmetric-numerical-method.md). Multiplication of the three [exponential](../../../../../../../matrix-exponential.md) series shows agreement with $e^{t(A+B)}$ through degree two. Equivalently, the [Baker--Campbell--Hausdorff formula](../../../../../../../baker-campbell-hausdorff-formula.md) gives an odd modified generator

$$
\log F(t)=t(A+B)+t^3D+O(t^5)
$$

for a matrix $D$ made from nested [commutators](../../../../../../../commutator.md). Exponentiating gives

$$
\boxed{F(t)=e^{t(A+B)}+Ct^3+O(t^4)}
$$

for a matrix $C$ depending on $A$ and $B$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Section A](../../../section-a.md)
4. [Paper 341](../../../../paper-341-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
