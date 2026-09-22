<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $s=|z|^2$. Contraction of the [symplectic form](../../../../../../symplectic-form.md) with the rotation [vector field](../../../../../../vector-field.md) gives

$$
\iota_K\omega=\frac{i}{(1+s)^2}\left(iz\,d\bar z+i\bar z\,dz\right)=-\frac{ds}{(1+s)^2}.
$$

With the convention fixed in the unheaded solution, $\iota_K\omega=-dH$, so **the [Hamiltonian function](../../../../../../hamiltonian-function.md) is**

$$
\boxed{H(z)=\frac{|z|^2}{1+|z|^2}+C.}
$$

Its derivative is $dH=ds/(1+s)^2$. In the chart $w=1/z$, $H=1/(1+|w|^2)+C$, so it extends smoothly across infinity; the additive constant is the kernel freedom already identified. Thus $K=X_H$ globally, proving that the action is a [Hamiltonian group action](../../../../../../hamiltonian-group-action.md). With $C=0$, the [moment map for rotation of the complex projective line](../../../../../../moment-map-for-rotation-of-the-complex-projective-line.md) takes values in $[0,1]$, reaching its endpoints at the two fixed poles.

One can check the normalization in polar coordinates: $\omega=2r(1+r^2)^{-2}dr\wedge d\phi$ has total [symplectic area](../../../../../../symplectic-area.md) $2\pi$, not $4\pi$, and $H=r^2/(1+r^2)$. Equivalently, in a polar angle with $r=\tan(\vartheta/2)$, $H=(1-\cos\vartheta)/2$. This explains the half-height factor that would be lost by replacing the printed form with the unscaled round-sphere area form. Under the opposite convention $\iota_{X_H}\omega=dH$, the Hamiltonian is the negative of this function, up to a constant.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
