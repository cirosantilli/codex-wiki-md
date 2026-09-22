<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the adjoint real bundle $\operatorname{ad}E$, the [ASD deformation complex](../../../../../../asd-deformation-complex.md) is

$$
\boxed{0\longrightarrow\Omega^0(\operatorname{ad}E)
\xrightarrow{\ d_A\ }\Omega^1(\operatorname{ad}E)
\xrightarrow{\ d_A^+\ }\Omega^{2,+}(\operatorname{ad}E)
\longrightarrow0,}
$$

where $d_A^+=P_+d_A$ and $P_+=(1+*)/2$. On an adjoint section $\xi$, the [vector-bundle curvature](../../../../../../curvature-form.md) identity gives $d_A^2\xi=[F_A,\xi]$. Since $P_+$ acts only on the two-form part and $F_A^+=0$,

$$
d_A^+d_A\xi=P_+[F_A,\xi]=[F_A^+,\xi]=0.
$$

This proves it is a complex. Its three [cohomology](../../../../../../cohomology-split.md) spaces are the infinitesimal stabilizers $H_A^0$, infinitesimal deformations modulo gauge $H_A^1$, and obstructions $H_A^2$.

The associated gauge-fixed [elliptic differential operator](../../../../../../elliptic-differential-operator.md) is

$$
D_A=d_A^*\oplus d_A^+:\Omega^1(\operatorname{ad}E)
\longrightarrow\Omega^0(\operatorname{ad}E)\oplus\Omega^{2,+}(\operatorname{ad}E).
$$

The [ASD deformation index](../../../../../../asd-deformation-index.md) formula is

$$
\begin{aligned}
\operatorname{ind}D_A
&=\dim H_A^1-\dim H_A^0-\dim H_A^2\\
&=-2\langle p_1(\operatorname{ad}E),[X]\rangle
-\frac32\bigl(\chi(X)+\sigma(X)\bigr)\\
&=8e(E)-3(1-b_1(X)+b^+(X)).
\end{aligned}
$$

Here the [Atiyah-Singer index theorem](../../../../../../atiyah-singer-index-theorem.md) is used for the formula, with $p_1(\operatorname{ad}E)=-4c_2(E)$ and $e(E)=c_2(E)[X]$. For the simply connected negative-definite base in this question, $b_1=b^+=0$, so **$\operatorname{ind}D_A=8e(E)-3$**. The alternating Euler characteristic of the three-term complex is the negative of this operator index; stating which index is being used avoids a sign ambiguity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
