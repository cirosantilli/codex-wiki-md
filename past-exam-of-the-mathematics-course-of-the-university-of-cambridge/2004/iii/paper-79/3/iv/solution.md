<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $z_r$ be either endpoint at which $Z_r$ is prescribed, and put $d_z=z-z_r$, $q=\mu p_\beta$ and $\kappa=\omega p_\beta$. Integrating the constant-coefficient [velocity](../../../../../../velocity.md)–[traction](../../../../../../traction.md) system gives

$$
\begin{pmatrix}V(z)\\T(z)\end{pmatrix}
=\begin{pmatrix}\cos\kappa d_z&-i\sin(\kappa d_z)/q\\-iq\sin\kappa d_z&\cos\kappa d_z\end{pmatrix}
\begin{pmatrix}V_r\\-Z_rV_r\end{pmatrix}.
$$

Taking the ratio $-T/V$ yields the [uniform-layer SH impedance update](../../../../../../uniform-layer-sh-impedance-update.md) and its accompanying [velocity](../../../../../../velocity.md):

$$
\boxed{Z(z)=\frac{Z_r\cos\kappa d_z+iq\sin\kappa d_z}{\cos\kappa d_z+i(Z_r/q)\sin\kappa d_z},\qquad
V(z)=V_r\left[\cos\kappa d_z+i\frac{Z_r}{q}\sin\kappa d_z\right].}
$$

The initial value $V_r$ sets an arbitrary normalization; specifying impedance alone cannot specify the overall wave [wave amplitude](../../../../../../wave-amplitude.md). Positive $d_z$ propagates data from $z_0$, while negative $d_z$ propagates a specified load from $z_1$, so the same expressions solve both requested initial-value problems.

Expanding sine and cosine gives

$$
\boxed{V(z)=\frac{V_r}{2}\left(1+\frac{Z_r}q\right)e^{i\kappa(z-z_r)}
+\frac{V_r}{2}\left(1-\frac{Z_r}q\right)e^{-i\kappa(z-z_r)}.}
$$

Absorbing the reference-point phases into the two constants gives the requested forward/backward exponential superposition. Equivalently, wherever the ratios are defined,

$$
\frac{Z(z)-q}{Z(z)+q}=\frac{Z_r-q}{Z_r+q}e^{-2i\kappa(z-z_r)}.
$$

The exceptional values $Z_r=q,-q$ give the pure directional solutions. If a denominator in the impedance formula vanishes, propagate the finite pair $(V,T)$ through that point; this is an impedance-chart pole, not a failure of the physical solution. The upper-half-plane assumptions ensure $q\ne0$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
