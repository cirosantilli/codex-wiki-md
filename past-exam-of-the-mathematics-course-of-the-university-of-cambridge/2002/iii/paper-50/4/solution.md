<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $a=\min(C_1,C_2)>0$, $b=\max(C_1,C_2)$ and $c=C^0>0$. At crystal orientation $\theta$, the conductivity [tensor](../../../../../tensor.md) is $Q_\theta\operatorname{diag}(a,b)Q_\theta^T$. Because the comparison [tensor](../../../../../tensor.md) is scalar, its resolvent rotates in the same way:

$$
M_\theta=[I+(C_\theta-cI)/(2c)]^{-1}
=Q_\theta\operatorname{diag}\left(\frac{2c}{a+c},\frac{2c}{b+c}\right)Q_\theta^T.
$$

Uniform angular averaging uses $\langle\cos^2\theta\rangle=\langle\sin^2\theta\rangle=1/2$ and $\langle\sin\theta\cos\theta\rangle=0$. It therefore sends any such rotated diagonal [tensor](../../../../../tensor.md) to half its trace times $I$. In particular,

$$
\langle M\rangle=c\left(\frac1{a+c}+\frac1{b+c}\right)I,
\qquad
\langle MC\rangle=c\left(\frac a{a+c}+\frac b{b+c}\right)I.
$$

Dividing these scalar coefficients in the stated [Hashin-Shtrikman conductivity variational principle](../../../../../hashin-shtrikman-conductivity-variational-principle.md) gives

$$
\boxed{C^{\mathrm{HS}}=H(c)I,\qquad H(c)=\frac{2ab+c(a+b)}{a+b+2c}.}
$$

This averaging calculation uses the uniform orientation model in the question; a nonuniform distribution need not give isotropic [effective conductivity](../../../../../effective-conductivity.md).

The lower [Hashin-Shtrikman conductivity bounds](../../../../../hashin-shtrikman-bounds-for-conductivity.md) use a comparison no larger than every local principal conductivity, so $0<c\le a$. The upper variational bound uses $c\ge b$. These opposite directions come from the sign of the contrast $C-cI$ in the polarization functional: positive contrast gives a maximizing lower principle, and negative contrast a minimizing upper principle. The endpoint values are understood as limits when a contrast eigenvalue vanishes. Since

$$
H'(c)=\frac{(a-b)^2}{(a+b+2c)^2}\ge0,
$$

the strongest lower and upper values in their admissible comparison ranges are, respectively,

$$
\boxed{C_l=H(a)=\frac{a(a+3b)}{3a+b},\qquad
C_u=H(b)=\frac{b(3a+b)}{a+3b}.}
$$

Thus $C_lI\preceq C^{\mathrm{eff}}\preceq C_uI$ in the statistically isotropic polycrystal setting of these [Hashin-Shtrikman conductivity bounds](../../../../../hashin-shtrikman-bounds-for-conductivity.md).

The [self-consistent conductivity approximation](../../../../../self-consistent-conductivity-approximation.md) chooses the comparison conductivity equal to the predicted conductivity, $c=C_{\mathrm{SC}}=H(c)$. Multiplication by the positive denominator cancels the terms $c(a+b)$ and leaves $2c^2=2ab$. Only the positive root is an admissible conductivity:

$$
\boxed{C_{\mathrm{SC}}=\sqrt{ab},\qquad C^{\mathrm{SC}}=\sqrt{ab}\,I.}
$$

For a direct proof of its ordering relative to the variational bounds, set $t=\sqrt{b/a}\ge1$. Then

$$
\frac{C_{\mathrm{SC}}-C_l}{a}=\frac{(t-1)^3}{t^2+3},
\qquad
\frac{C_u-C_{\mathrm{SC}}}{a}=\frac{t(t-1)^3}{1+3t^2}.
$$

Both quantities are nonnegative, proving **$C_l\le C_{\mathrm{SC}}\le C_u$**, with equality throughout when $a=b$. The [self-consistent conductivity approximation](../../../../../self-consistent-conductivity-approximation.md) is a closure calculation; no unrequested claim of exactness for every spatial arrangement follows just from this fixed-point computation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
