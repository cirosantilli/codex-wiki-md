<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [smooth exponential sequence](../../../../../smooth-exponential-sequence.md) is

$$
0\longrightarrow\underline{\mathbb Z}\longrightarrow
\mathcal C^\infty(\mathbb C)
\xrightarrow{\exp(2\pi i\,\cdot)}
\mathcal C^\infty(\mathbb C^\times)\longrightarrow1.
$$

Local logarithms make it exact as a sequence of sheaves. A [line bundle](../../../../../line-bundle.md) has a transition class in $H^1(M,\mathcal C^\infty(\mathbb C^\times))$; its image under the connecting map defines the [First Chern class](../../../../../first-chern-class.md). For a holomorphic [line bundle](../../../../../line-bundle.md) the holomorphic exponential sequence gives the same class by naturality.

Here is the explicit [Čech-de Rham curvature descent](../../../../../cech-de-rham-curvature-descent.md). On a good cover, write $e_j=e_i g_{ij}$ and choose logarithms $g_{ij}=\exp(2\pi i f_{ij})$. The integer cocycle

$$
c_{ijk}=f_{ij}+f_{jk}-f_{ik}
$$

represents $c_1(E)$. By the proved frame formula,

$$
A_j-A_i=2\pi i\,df_{ij}.
$$

Put $B_i=-A_i/(2\pi i)$ and $F=i\Theta/(2\pi)=dB_i$. Then $\delta B=-df$ and $\delta f=c$. In the [Čech-de Rham double complex](../../../../../cech-de-rham-double-complex.md), with total differential $D_{\mathrm{tot}}=\delta+(-1)^p d$ on Čech degree $p$,

$$
D_{\mathrm{tot}}B=F-df,\qquad
D_{\mathrm{tot}}f=c-df,\qquad
F-c=D_{\mathrm{tot}}(B-f).
$$

Thus the global [closed differential form](../../../../../closed-differential-form.md) and the integer cocycle represent the same class under [de Rham theorem](../../../../../de-rham-theorem.md):

$$
\boxed{\left[\frac{i}{2\pi}\Theta\right]=c_1(E)_{\mathbb C}.}
$$

This proves integrality, including the sign and normalization. It identifies the image of the integral class; [vector-bundle curvature](../../../../../curvature-form.md) alone cannot recover torsion classes lost in passage to complex coefficients.

Two connections on the same [line bundle](../../../../../line-bundle.md) differ by a global scalar one-form $a$. Their [vector-bundle curvatures](../../../../../curvature-form.md) satisfy $\Theta_1-\Theta=da$, so the normalized representatives differ by an [exact differential form](../../../../../exact-differential-form.md). Hence the class is independent of the connection.

Use the integral normalization of the [Fubini-Study form](../../../../../fubini-study-form.md). On the chart $Z_j\ne0$, define the [integrally normalized Fubini-Study form](../../../../../integrally-normalized-fubini-study-form.md) by

$$
\boxed{\omega_{\mathrm{int}}=\frac{i}{2\pi}\partial\bar\partial
\log\!\left(\frac{\sum_{k=0}^n|Z_k|^2}{|Z_j|^2}\right).}
$$

The potentials on overlaps differ by the logarithm of the squared modulus of a nowhere-zero holomorphic function, whose $\partial\bar\partial$ is zero. Thus the forms patch and are closed. The dual of the tautological metric on $\mathcal O(1)$ has local squared norm $h=(1+\sum|z_k|^2)^{-1}$. Its [Chern connection](../../../../../chern-connection.md) has $A=\partial\log h$ and [vector-bundle curvature](../../../../../curvature-form.md) $\Theta=\bar\partial\partial\log h=\partial\bar\partial\log(1+\sum|z_k|^2)$. Therefore **$[\omega_{\mathrm{int}}]=c_1(\mathcal O(1))$**, proving the requested integrality. With the unnormalized convention $\omega_{FS}=i\partial\bar\partial\log(1+\sum|z_k|^2)$, this is $\omega_{\mathrm{int}}=\omega_{FS}/(2\pi)$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
