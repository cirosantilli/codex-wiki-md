<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work entirely with left-handed [Weyl fermions](../../../../weyl-spinor.md); a right-handed field is counted through its left-handed charge conjugate. For a simple non-Abelian group $G$, define

$$
\operatorname{tr}_{R}(T^aT^b)=T(R)\delta^{ab},\qquad
D_R^{abc}=\operatorname{tr}_{R}[T^a\{T^b,T^c\}].
$$

The two orientations of a chiral triangle supply the symmetrized [trace](../../../../matrix-trace.md). Spectator representation dimensions multiply each [trace](../../../../matrix-trace.md). The perturbative [gauge anomaly](../../../../gauge-anomaly.md) conditions for $G\times U(1)$ are therefore

$$
\boxed{\sum_iD_{R_i}^{abc}=0\quad\text{for every }a,b,c,\qquad
\sum_iQ_iT(R_i)=0,\qquad
\sum_i\dim(R_i)Q_i^3=0.}
$$

The first concerns $G^3$, the second $G^2U(1)$, and the third $U(1)^3$. A $GU(1)^2$ triangle has group factor $\sum_iQ_i^2\operatorname{tr}_{R_i}T^a=0$, because non-Abelian generators of a semisimple group are traceless. If coupling to gravity is required, also impose the mixed gauge-gravitational condition $\sum_i\dim(R_i)Q_i=0$. Cancellation of these local triangles is not a universal substitute for checking global anomalies; the [Witten SU(2) anomaly](../../../../witten-su-2-anomaly.md) is the relevant additional test here.[§§3.4.1–3.4.4: local gauge anomalies, mixed gravitational condition, [SU(2)](../../../../su-2-group.md) [global anomaly](../../../../global-anomaly.md) and [Standard Model](../../../../standard-model-split.md)](../../../../gauge-theory-by-david-tong.md)

For the [Standard Model](../../../../standard-model-split.md), one generation consists of $Q_L:(3,2)_{1/6}$, $u^c:(\bar3,1)_{-2/3}$, $d^c:(\bar3,1)_{1/3}$, $L_L:(1,2)_{-1/2}$ and $e^c:(1,1)_1$. These are precisely the all-left-handed representations; conjugating the singlets reverses their [hypercharges](../../../../hypercharge.md) relative to right-handed [particles](../../../../particle-physics.md). Check the requested triangles separately:

For $3$–$3$–$3$, normalize the cubic coefficient of a fundamental to $+1$. Its conjugate has $-1$, so the weak-doublet multiplicity gives

$$
\mathcal A_{333}=2-1-1=0.
$$

For $2$–$2$–$2$, the doublet generators obey $\{T^b,T^c\}=\delta^{bc}I/2$, so $\operatorname{tr}(T^a\{T^b,T^c\})=0$. Thus every doublet separately has zero local cubic weak anomaly. For the global [Witten SU(2) anomaly](../../../../witten-su-2-anomaly.md), each generation has three coloured [quark](../../../../quark.md) doublets and one lepton doublet, an even total of four. All three generations give twelve, so the global obstruction also cancels.

For $3$–$3$–$1$, use $T(3)=T(\bar3)=1/2$. The two conjugate triplets have the same quadratic index, not its negative:

$$
\mathcal A_{331}=2\left(\frac16\right)\frac12
+\left(-\frac23\right)\frac12
+\left(\frac13\right)\frac12=0.
$$

For $2$–$2$–$1$, the three [quark](../../../../quark.md) colours and one lepton doublet give

$$
\mathcal A_{221}=3\left(\frac16\right)\frac12
+\left(-\frac12\right)\frac12=0.
$$

For $1$–$1$–$1$, count every coloured and weak component:

$$
\mathcal A_{111}=6\left(\frac16\right)^3+3\left(-\frac23\right)^3
+3\left(\frac13\right)^3+2\left(-\frac12\right)^3+1
=\frac{1-32+4-9+36}{36}=0.
$$

The mixed gauge-gravitational coefficient also vanishes:

$$
6\left(\frac16\right)+3\left(-\frac23\right)+3\left(\frac13\right)
+2\left(-\frac12\right)+1=0.
$$

Unlisted gauge combinations contain a single generator of at least one simple factor. For example, $3$–$2$–$1$ has $\operatorname{tr}_3T^a\operatorname{tr}_2t^b\,Y$, and $3$–$3$–$2$ has $\operatorname{tr}_3(T^aT^b)\operatorname{tr}_2t^c$; both vanish. The same reasoning covers $3$–$1$–$1$, $2$–$1$–$1$ and $3$–$2$–$2$, including permutations of the legs. [Scalars](../../../../scalar.md) contribute no chiral triangle anomaly. Therefore

$$
\boxed{\text{All the listed gauge anomalies cancel within each generation; three generations remain anomaly free.}}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
