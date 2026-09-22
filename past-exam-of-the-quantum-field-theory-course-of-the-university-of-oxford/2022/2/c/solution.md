<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $u_i=u^{s_i}(p_i)$ and $v_i=v^{s_i}(p_i)$. With $S_{fi}=\delta_{fi}+i(2\pi)^4\delta^{(4)}(p_1+p_2-p_3-p_4)\mathcal M_{fi}$, choose

$$
\boxed{\mathcal M_{p_1,p_2,p_3,p_4}^{s_1,s_2,s_3,s_4}=g^2(T-A),\qquad
T=(\bar u_3u_1)(\bar v_2v_4),\quad A=(\bar v_2u_1)(\bar u_3v_4).}
$$

The relative minus sign is fixed by the [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md), not by the [Mandelstam variables](../../../../mandelstam-variables.md). It follows by [crossing symmetry](../../../../crossing-symmetry.md) from the identical-[fermion](../../../../fermion.md) [scattering amplitude](../../../../scattering-amplitude.md) in [i](../b/i.md), or directly by the two inequivalent external contractions of $g^2(\bar\psi\psi)^2/2$. For an explicit sign check, fix incoming state order $b_1^\dagger d_2^\dagger|0\rangle$ and outgoing order $b_3^\dagger d_4^\dagger|0\rangle$. The direct contraction contains $(b_3^\dagger b_1)(d_2d_4^\dagger)$, whose coefficient in the ordered product $b_3^\dagger d_4^\dagger d_2b_1$ is $-1$; the annihilation contraction $(b_3^\dagger d_4^\dagger)(d_2b_1)$ has coefficient $+1$. The common sign can change with the external-state convention, while their relative minus sign cannot.

Let $r=m^2$. The external particles are [on shell](../../../../on-shell.md), so $s+t+u=4r$ and

$$
p_1\cdot p_2=p_3\cdot p_4=\frac s2-r,\qquad
p_1\cdot p_3=p_2\cdot p_4=r-\frac t2,\qquad
p_1\cdot p_4=p_2\cdot p_3=r-\frac u2.
$$

Use the supplied [spin sums](../../../../spin-sum.md) and [gamma matrix trace identities](../../../../gamma-matrix-trace-identities.md). The two diagonal terms in the initial [spin average](../../../../spin-average.md) are

$$
\frac14\sum|T|^2
=\frac14\operatorname{Tr}[(\not p_3+m)(\not p_1+m)]
\operatorname{Tr}[(\not p_2-m)(\not p_4-m)]
=(t-4r)^2,
$$



$$
\frac14\sum|A|^2
=\frac14\operatorname{Tr}[(\not p_2-m)(\not p_1+m)]
\operatorname{Tr}[(\not p_3+m)(\not p_4-m)]
=(s-4r)^2.
$$

For the interference term, the [spin sum](../../../../spin-sum.md) is a single [Dirac trace](../../../../gamma-matrix-trace.md):

$$
R:=\sum TA^*
=\operatorname{Tr}[(\not p_3+m)(\not p_1+m)(\not p_2-m)(\not p_4-m)].
$$

Terms with an odd number of [Dirac gamma matrices](../../../../gamma-matrices.md) vanish. Expanding the remaining terms gives

$$
\begin{aligned}
\frac R4={}&(p_3\cdot p_1)(p_2\cdot p_4)
-(p_3\cdot p_2)(p_1\cdot p_4)
+(p_3\cdot p_4)(p_1\cdot p_2)\\
&+r(p_3\cdot p_1-p_3\cdot p_2-p_3\cdot p_4-p_1\cdot p_2-p_1\cdot p_4+p_2\cdot p_4)+r^2.
\end{aligned}
$$

Substituting the [Mandelstam variables](../../../../mandelstam-variables.md) reduces this to

$$
R=s^2+t^2-u^2+16ru-16r^2
=(s-4r)^2+(t-4r)^2-(u-4r)^2.
$$

It is real. The initial [spin average](../../../../spin-average.md) therefore yields

$$
\overline{|\mathcal M|^2}=g^4\left[(t-4r)^2+(s-4r)^2-\frac R2\right],
$$



$$
\boxed{\overline{|\mathcal M|^2}=\frac{g^4}{2}\left[(s-4m^2)^2+(t-4m^2)^2+(u-4m^2)^2\right].}
$$

**The displayed answer in the source is false.** At threshold, $p_i=(m,\mathbf0)$, hence $s=4m^2$ and $t=u=0$. Then $\bar vu=\bar uv=0$, while the [spin sums](../../../../spin-sum.md) give $\overline{|\mathcal M|^2}=16g^4m^4$. The printed expression instead gives $20g^4m^4$. This is also a counterexample in the continuous threshold limit from physical nonzero incoming [momenta](../../../../momentum-split.md). At $m=0$ there is a further discrepancy: the correct result is $g^4(s^2+t^2+u^2)/2$, rather than the printed $g^4(3s^2+3t^2-u^2)/2$. Changing a common phase of the [scattering amplitude](../../../../scattering-amplitude.md) cannot change either comparison.

The requested $s\leftrightarrow t$ symmetry nevertheless holds for the correct answer. [Crossing symmetry](../../../../crossing-symmetry.md) exchanges the two ways of pairing the four external [fermion](../../../../fermion.md) lines; the momentum-independent [auxiliary-field propagator](../../../../auxiliary-field-propagator.md) supplies no channel-dependent denominator. The relative [fermionic sign](../../../../fermionic-sign.md) can reverse the crossed [scattering amplitude](../../../../scattering-amplitude.md), but disappears in its squared modulus. With $u=4m^2-s-t$, the boxed expression is manifestly symmetric under $s\leftrightarrow t$. This is an analytic crossing relation, not a statement that positive physical $s$ and negative physical $t$ have interchangeable scattering kinematics.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
