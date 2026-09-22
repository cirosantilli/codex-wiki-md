<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By the [monoidal coherence theorem](../../../../../../monoidal-coherence-theorem.md), calculations may suppress the canonical [associators](../../../../../../associator.md) and [unitors](../../../../../../unitor.md), restoring them uniquely afterwards. In this notation the two [Frobenius monoidal functor](../../../../../../frobenius-monoidal-functor.md) identities read

$$
\psi_{A\otimes B,C}\varphi_{A,B\otimes C}=(\varphi_{A,B}\otimes1)(1\otimes\psi_{B,C}),
$$



$$
\psi_{A,B\otimes C}\varphi_{A\otimes B,C}=(1\otimes\varphi_{B,C})(\psi_{A,B}\otimes1).
$$

Write

$$
E=\psi_0F(e)\varphi_{X,Y},\qquad N=\psi_{Y,X}F(n)\varphi_0.
$$

We check both [snake identities](../../../../../../snake-identity.md) for this prospective [dual pair in a monoidal category](../../../../../../dual-pair-in-a-monoidal-category.md). For $FX$, expand and use the first Frobenius identity:

$$
\begin{aligned}
(E\otimes1)(1\otimes N)&=(\psi_0\otimes1)(Fe\otimes1)(\varphi_{X,Y}\otimes1)(1\otimes\psi_{Y,X})(1\otimes Fn)(1\otimes\varphi_0)\\
&=(\psi_0\otimes1)(Fe\otimes1)\psi_{X\otimes Y,X}\varphi_{X,Y\otimes X}(1\otimes Fn)(1\otimes\varphi_0)\\
&=(\psi_0\otimes1)\psi_{I,X}F(e\otimes1)F(1\otimes n)\varphi_{X,I}(1\otimes\varphi_0)\\
&=1_{FX}.
\end{aligned}
$$

The third line uses [naturality](../../../../../../naturality.md) of $\psi$ and $\varphi$. The last line uses $(e\otimes1)(1\otimes n)=1_X$, followed by the opmonoidal and monoidal unit axioms.

For $FY$, the second Frobenius identity gives the other calculation:

$$
\begin{aligned}
(1\otimes E)(N\otimes1)&=(1\otimes\psi_0)(1\otimes Fe)(1\otimes\varphi_{X,Y})(\psi_{Y,X}\otimes1)(Fn\otimes1)(\varphi_0\otimes1)\\
&=(1\otimes\psi_0)(1\otimes Fe)\psi_{Y,X\otimes Y}\varphi_{Y\otimes X,Y}(Fn\otimes1)(\varphi_0\otimes1)\\
&=(1\otimes\psi_0)\psi_{Y,I}F(1\otimes e)F(n\otimes1)\varphi_{I,Y}(\varphi_0\otimes1)\\
&=1_{FY}.
\end{aligned}
$$

Thus **both triangular identities hold**, and

$$
\boxed{E:FX\otimes FY\to I,\qquad N:I\to FY\otimes FX}
$$

are the [evaluation morphism](../../../../../../evaluation-morphism.md) and [coevaluation morphism](../../../../../../coevaluation-morphism.md) of a [dual pair in a monoidal category](../../../../../../dual-pair-in-a-monoidal-category.md). Notice that none of the comparison maps was assumed invertible.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
