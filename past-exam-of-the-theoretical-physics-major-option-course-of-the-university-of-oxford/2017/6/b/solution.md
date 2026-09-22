<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For this [three-site Abelian Higgs chain](../../../../three-site-abelian-higgs-chain.md), the potential is minimized by $|\phi_1|=|\phi_2|=v$. Choose their phases real in a local [unitary gauge](../../../../unitary-gauge.md). The scalar [kinetic terms](../../../../kinetic-term.md) then give

$$
\mathcal L_{\mathrm{mass}}=g^2v^2\left[(B^1-qB^2)^2+(B^2-qB^3)^2\right]
=g^2v^2B^{\mathsf T}KB,
$$

where Lorentz contractions are understood and

$$
K=R^{\mathsf T}R=\begin{pmatrix}1&-q&0\\-q&1+q^2&-q\\0&-q&q^2\end{pmatrix},\qquad
R=\begin{pmatrix}1&-q&0\\0&1&-q\end{pmatrix}.
$$

The nonzero [eigenvalues](../../../../eigenvalue.md) of $K$ equal those of

$$
RR^{\mathsf T}=\begin{pmatrix}1+q^2&-q\\-q&1+q^2\end{pmatrix},
$$

namely $1+q^2-q$ and $1+q^2+q$. The third [eigenvalue](../../../../eigenvalue.md) is zero because $R$ has rank two. Both nonzero [eigenvalues](../../../../eigenvalue.md) are positive for $q>0$.

**Mass-normalization correction:** the canonical vector [mass](../../../../mass.md) term is $\tfrac12B^{\mathsf T}\mathsf M^2B$, so the [Lagrangian](../../../../lagrangian.md) actually gives $\mathsf M^2=2g^2v^2K$. Its physical [masses](../../../../mass.md) are therefore

$$
\boxed{m_1=0,\qquad m_2=\sqrt2gv\sqrt{q^2-q+1},\qquad
m_3=\sqrt2gv\sqrt{q^2+q+1}.}
$$

The printed dimensionless [eigenvalue](../../../../eigenvalue.md) pattern is correct, but its common scale must be $m=\sqrt2gv$, not $gv$, for the written [kinetic terms](../../../../kinetic-term.md) and [vacuum](../../../../vacuum.md) value. For a concrete counterexample set $q=1$ and $B=(A,0,-A)/\sqrt2$. This is a canonically normalized eigenmode and its [mass](../../../../mass.md) term is $g^2v^2A_\mu A^\mu$, giving physical squared [mass](../../../../mass.md) $2g^2v^2$ rather than the printed $g^2v^2$. The printed scale $gv$ would require a [vacuum](../../../../vacuum.md) modulus $v/\sqrt2$ or a corresponding change in scalar normalization, neither of which is the specified potential minimum.

The unbroken transformations preserve both [vacuum](../../../../vacuum.md) phases:

$$
\alpha_1-q\alpha_2=0,\qquad\alpha_2-q\alpha_3=0,
\qquad (\alpha_1,\alpha_2,\alpha_3)=\alpha(q^2,q,1).
$$

Thus the local breaking pattern is

$$
\boxed{U(1)^3\longrightarrow U(1).}
$$

Two scalar phases supply the longitudinal [polarizations](../../../../polarization-waves.md) of the two massive [vector bosons](../../../../vector-boson.md); one massless vector remains. This is the [Higgs mechanism](../../../../higgs-mechanism.md), with its [mass](../../../../mass.md) [matrix](../../../../matrix.md) fixed by the scalar charge [matrix](../../../../matrix.md) and the [vacuum](../../../../vacuum.md) normalization.[Section 2.5.2, expanding scalar kinetic terms around a condensate to obtain a vector mass](../../../../gauge-theory-by-david-tong.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
