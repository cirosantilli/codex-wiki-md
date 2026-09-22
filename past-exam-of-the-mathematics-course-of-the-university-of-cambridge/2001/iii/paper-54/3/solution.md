<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The spatial [reflection](../../../../../reflection-mathematics.md) $x\mapsto-x$ acts on the two complex [amplitudes](../../../../../wave-amplitude.md) as $(A,B)\mapsto(A,-B)$, because the first spatial [eigenfunction](../../../../../eigenfunction.md) is even and the second is odd. The first equation must therefore be even in $B,\overline B$, and the second odd. For a nonresonant double [Hopf bifurcation](../../../../../hopf-bifurcation.md), the temporal [phases](../../../../../phase-waves.md) give independent actions $A\mapsto e^{i\varphi_1}A$, $B\mapsto e^{i\varphi_2}B$ in the cubic [normal form of a dynamical system](../../../../../normal-form-dynamical-systems.md). A cubic [monomial](../../../../../monomial.md) in the first equation must have net $A$ [phase](../../../../../phase-waves.md) weight one and net $B$ [phase](../../../../../phase-waves.md) weight zero. Only $A|A|^2,A|B|^2$ satisfy this; the second equation similarly has $B|B|^2,B|A|^2$. Parametrizing the independent cross-saturation [coefficients](../../../../../coefficient.md) gives

$$
\begin{aligned}
\dot A&=\nu_1A-\alpha_1(|A|^2+|B|^2)A-\beta_1|B|^2A,\\
\dot B&=\nu_2B-\alpha_2(|A|^2+|B|^2)B-\beta_2|A|^2B.
\end{aligned}
$$

All [coefficients](../../../../../coefficient.md) can be complex: their [real parts](../../../../../real-part.md) determine [amplitude](../../../../../wave-amplitude.md) growth and their [imaginary parts](../../../../../imaginary-part.md) frequency shifts. These are cubic truncations of a family of reduced vector fields on the four-real-dimensional [extended centre manifold](../../../../../extended-centre-manifold-for-a-parameter.md), with the two unfolding parameters entering $\nu_1,\nu_2$.

The nonresonance assumption must be made explicit. Merely having $\omega_1\ne\omega_2$ does not imply this form: for $\omega_1=2\omega_2$, the quadratic terms $B^2$ in $\dot A$ and $A\overline B$ in $\dot B$ satisfy both temporal [resonance](../../../../../resonance.md) and spatial parity. Thus the initial form is the generic nonresonant double-Hopf form, rather than a statement for every possible unequal frequency pair.

At the one-to-one [reflection-symmetric one-to-one Hopf resonance](../../../../../reflection-symmetric-one-to-one-hopf-resonance.md), only the common temporal [phase](../../../../../phase-waves.md) action remains. Cubic terms must then have total [phase](../../../../../phase-waves.md) weight one. Spatial [reflection](../../../../../reflection-mathematics.md) retains, in the first equation, the three terms $A|A|^2,A|B|^2,B^2\overline A$; the second retains $B|B|^2,B|A|^2,A^2\overline B$. Common [phase](../../../../../phase-waves.md) covariance excludes all quadratic terms. The additional resonant terms are consequently $-\gamma_1B^2\overline A$ and $-\gamma_2A^2\overline B$, with independent complex [coefficients](../../../../../coefficient.md). This is the [reflection-symmetric one-to-one Hopf resonance](../../../../../reflection-symmetric-one-to-one-hopf-resonance.md).

In the specified equal-coefficient specialization, put $r=R^2$. A nonzero pure-$A$ periodic branch exists for $\operatorname{Re}\nu_1>0$ and has

$$
r=\frac{\operatorname{Re}\nu_1}{\alpha_R},\qquad
\Omega=\operatorname{Im}\nu_1-\alpha_Ir.
$$

Its radial [eigenvalue](../../../../../eigenvalue.md) is $-2\alpha_Rr<0$, and its [phase](../../../../../phase-waves.md) is neutral. For a transverse $B$ perturbation the linear equation is

$$
\dot B=[\nu_2-(\alpha+\beta)r]B-\beta r e^{2i\Omega t}\overline B.
$$

Its time dependence can be removed exactly by $B=C e^{i\Omega t}$. Using $\nu_1-\alpha r=i\Omega$ and $\nu_2=\nu_1-d$ gives

$$
\boxed{\dot C=-(d+\beta r)C-\beta r\overline C.}
$$

Writing $C=u+iv$, $d=d_R+id_I$, $\beta=\beta_R+i\beta_I$ yields the constant real [stability matrix](../../../../../stability-matrix.md)

$$
M(r)=\begin{pmatrix}-d_R-2\beta_Rr&d_I\\-d_I-2\beta_Ir&-d_R\end{pmatrix}.
$$

Let $Q=\operatorname{Re}(\beta\overline d)=\beta_Rd_R+\beta_Id_I$. The transverse [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\boxed{\lambda^2+2(d_R+\beta_Rr)\lambda+|d|^2+2rQ=0.}
$$

Both transverse [eigenvalues](../../../../../eigenvalue.md) have negative [real part](../../../../../real-part.md) exactly when

$$
d_R+\beta_Rr>0,\qquad |d|^2+2rQ>0.
$$

These hold at $r=0$ because $d_R>0$. Thus a sufficiently small pure branch is transversely stable; it is stable modulo its neutral temporal [phase](../../../../../phase-waves.md) until one of the two inequalities fails. The [secondary steady and Hopf thresholds of a resonant pure mode](../../../../../secondary-steady-and-hopf-thresholds-of-a-resonant-pure-mode.md) are derived in the two parts below. They refer to accessible points on the pure branch; in a multi-parameter problem $d$ may also vary, so a proposed parameter path must actually cross the corresponding surface.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
