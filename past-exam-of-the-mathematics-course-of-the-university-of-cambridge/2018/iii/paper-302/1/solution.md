<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [Matrix Lie group](../../../../../matrix-lie-group.md), the [exponential map of a matrix Lie group](../../../../../exponential-map-of-a-matrix-lie-group.md) is the convergent [matrix exponential](../../../../../matrix-exponential.md)

$$
\boxed{\operatorname{Exp}(X)=e^X=\sum_{n=0}^{\infty}\frac{X^n}{n!}.}
$$

Its domain is the [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak g=T_I G$, and $e^{tX}\in G$ for every real $t$ when $X\in\mathfrak g$. Because multiples of the same matrix commute, $e^{sX}e^{tX}=e^{(s+t)X}$ and $(e^{tX})^{-1}=e^{-tX}$. Thus take $I=\mathbb R$ to obtain the image of a [one-parameter subgroup](../../../../../one-parameter-subgroup.md).

Here is the precise [classification of nontrivial one-parameter subgroups](../../../../../classification-of-nontrivial-one-parameter-subgroups.md). For $X\ne0$, the smooth [group homomorphism](../../../../../group-homomorphism.md) $\gamma_X:t\mapsto e^{tX}$ has a closed kernel $K\subset\mathbb R$. A closed subgroup of $\mathbb R$ is zero, $\tau\mathbb Z$ for some $\tau>0$, or all of $\mathbb R$. Indeed, if positive elements have infimum zero, their integer multiples approximate every real number, so closedness makes the subgroup all of $\mathbb R$; otherwise the infimum is attained and is its least positive generator. The last possibility is excluded by $\gamma_X'(0)=X\ne0$. Give the image the quotient topology and smooth structure from $\mathbb R/K$. Its inclusion in $G$ is an injective [immersion](../../../../../immersion.md), since $\gamma_X'(t)=e^{tX}X$ never vanishes. Consequently it is a [Lie subgroup](../../../../../lie-subgroup.md), with

$$
\boxed{G_X\cong(\mathbb R,+)\quad\text{or}\quad\mathbb R/(\tau\mathbb Z)\cong S^1.}
$$

In the periodic case $[0,\tau)$ is also a parameter interval covering the image, with endpoints understood modulo $\tau$.

Two qualifications matter. If $X=0$, the image is the trivial group, a third possibility omitted by the wording “two”. Also, a general [one-parameter subgroup](../../../../../one-parameter-subgroup.md) need not be closed or embedded: an irrational winding $t\mapsto\operatorname{diag}(R(t),R(\sqrt2t))$ in a two-torus is an example, where $R(t)$ is a planar rotation. The classification uses the intrinsic immersed [Lie subgroup](../../../../../lie-subgroup.md) structure, rather than assuming that the matrix subspace topology is the topology of $\mathbb R$.

For the real [special linear group](../../../../../special-linear-group.md), differentiating $\det(I+tX)=1+t\operatorname{tr}X+O(t^2)$ at the identity shows that its Lie algebra consists of traceless matrices. Conversely $\det e^{tX}=e^{t\operatorname{tr}X}=1$ for a traceless matrix. Hence

$$
\boxed{\mathfrak{sl}_2(\mathbb R)=\left\{\begin{pmatrix}a&b\\c&-a\end{pmatrix}:a,b,c\in\mathbb R\right\}.}
$$

Choose the standard basis of the real [sl2 Lie algebra](../../../../../sl2-lie-algebra.md),

$$
L_0=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad
L_+=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad
L_-=\begin{pmatrix}0&0\\1&0\end{pmatrix}.
$$

Their squares have the required values. Direct matrix multiplication gives the [Lie brackets](../../../../../lie-bracket.md)

$$
\boxed{[L_0,L_+]=2L_+,\qquad[L_0,L_-]=-2L_-,\qquad[L_+,L_-]=L_0.}
$$

Writing $[L_a,L_b]=f_{ab}{}^cL_c$, these specify all the nonzero [Lie algebra structure constants](../../../../../structure-constant-of-a-lie-algebra.md): $f_{0+}{}^+=2$, $f_{0-}{}^-=-2$, $f_{+-}{}^0=1$, together with their negatives on reversing the lower indices.

The three requested exponentials are

$$
\begin{aligned}
e^{tL_0}&=\begin{pmatrix}e^t&0\\0&e^{-t}\end{pmatrix},&&t\in\mathbb R,\\
e^{tL_+}&=I_2+tL_+=\begin{pmatrix}1&t\\0&1\end{pmatrix},&&t\in\mathbb R,\\
e^{t(L_+-L_-)}&=\begin{pmatrix}\cos t&\sin t\\-\sin t&\cos t\end{pmatrix},&&t\in[0,2\pi).
\end{aligned}
$$

Thus the first two images are isomorphic to the additive real group, while the last is $SO(2)$, the [circle group](../../../../../circle-group.md). The PDF gives $L_+-L_-$ here; the local TeX's $L_--L_-$ is a transcription error.

For a general generator, put $\Delta=\alpha_0^2+\alpha_+\alpha_-$. Direct multiplication gives $X^2=\Delta I_2$. If $\Delta>0$, the eigenvalues $\pm\sqrt\Delta$ give an unbounded exponential image. If $\Delta=0$ but $X\ne0$, it is a [nilpotent linear map](../../../../../nilpotent-linear-map.md) with exponential $I_2+tX$, again unbounded. If $\Delta=-\omega^2<0$, the power series instead gives

$$
e^{tX}=\cos(\omega t)I_2+\frac{\sin(\omega t)}\omega X,
$$

with least positive period $2\pi/\omega$. Its image is a continuous image of a circle and is compact. Equivalently, $X/\omega$ is a real complex structure and is similar over $\mathbb R$ to the rotation generator. Therefore the exact criterion for [compact one-parameter subgroups of SL2R](../../../../../compact-one-parameter-subgroups-of-sl2r.md) is

$$
\boxed{G_X\text{ is compact}\quad\Longleftrightarrow\quad\alpha_0^2+\alpha_+\alpha_-<0\ \text{or}\ (\alpha_0,\alpha_+,\alpha_-)=(0,0,0).}
$$

For a nonzero generator only the strict inequality remains.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
