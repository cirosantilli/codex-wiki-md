<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In [conformal gauge](../../../../../conformal-gauge.md), a free [closed bosonic string](../../../../../closed-string.md) has $(\partial_\tau^2-\partial_\sigma^2)X^\mu=0$, periodicity in $\sigma$, and the two [Virasoro constraints](../../../../../virasoro-constraint.md) $(\dot X\pm X')^2=0$. Its left- and right-moving [string oscillator](../../../../../string-oscillator.md) families have independent [Virasoro generators](../../../../../virasoro-generator.md) $L_n$ and $\widetilde L_n$. In [old covariant string quantization](../../../../../old-covariant-string-quantization.md), a [physical string state](../../../../../physical-string-state.md) obeys

$$
L_{n>0}|\Phi\rangle=\widetilde L_{n>0}|\Phi\rangle=0,
\qquad
(L_0-a)|\Phi\rangle=(\widetilde L_0-a)|\Phi\rangle=0,
$$

with $a=1$ in the critical [bosonic string theory](../../../../../bosonic-string-theory.md). The two zero-mode conditions also impose [closed-string level matching](../../../../../closed-string-level-matching.md). For an [open string](../../../../../open-string.md), keep just one [string oscillator](../../../../../string-oscillator.md) family. Negative-mode constraints are adjoints on bras, not additional annihilation conditions on [physical string states](../../../../../physical-string-state.md).

A [spurious string state](../../../../../spurious-string-state.md) is a [Virasoro descendant](../../../../../virasoro-descendant.md) orthogonal to every [physical string state](../../../../../physical-string-state.md): if $|s\rangle=\sum_{n>0}L_{-n}|\chi_n\rangle$, then $\langle\Phi|s\rangle=0$ follows from $L_n|\Phi\rangle=0$ and $L_n^\dagger=L_{-n}$. A [null string state](../../../../../null-string-state.md) is a spurious state that is itself physical. It consequently has zero norm and is removed in the [null-state quotient of a string](../../../../../null-state-quotient-of-a-string.md). The calculations below concern one [string oscillator](../../../../../string-oscillator.md) family and use

$$
[L_m,L_n]=(m-n)L_{m+n}+\frac d{12}(m^3-m)\delta_{m+n,0},
\qquad [L_m,\alpha_n^\mu]=-n\alpha_{m+n}^\mu.
$$

For $|n_1\rangle=L_{-1}|\chi_1\rangle$ with $L_0|\chi_1\rangle=0$ and all positive modes zero, $L_0|n_1\rangle=|n_1\rangle$. Also

$$
L_1|n_1\rangle=2L_0|\chi_1\rangle=0,
\qquad
L_m|n_1\rangle=(m+1)L_{m-1}|\chi_1\rangle=0\quad(m\geq2).
$$

It is therefore physical for [string intercept](../../../../../normal-ordering-constant-of-a-string.md) one and spurious by construction. In particular $\|n_1\|^2=\langle\chi_1|2L_0|\chi_1\rangle=0$. This proves the requested level-one descendant is null.

For the scalar descendant, write $|v_b\rangle=(L_{-2}+bL_{-1}^2)|\chi_2\rangle$ with $L_0|\chi_2\rangle=-|\chi_2\rangle$ and positive modes zero. Direct commutation gives

$$
L_0|v_b\rangle=|v_b\rangle,
\qquad
L_1|v_b\rangle=(3-2b)L_{-1}|\chi_2\rangle,
\qquad
L_2|v_b\rangle=\left(\frac d2-4-6b\right)|\chi_2\rangle.
$$

For instance $[L_1,L_{-1}^2]|\chi_2\rangle=-2L_{-1}|\chi_2\rangle$ and $L_2L_{-1}^2|\chi_2\rangle=-6|\chi_2\rangle$. Modes $m\geq3$ annihilate $|v_b\rangle$ because every remaining positive mode annihilates its parent. Hence the physical scalar descendant requires $b=3/2$ and $d=26$:

$$
\boxed{|n_2\rangle=\left(L_{-2}+\frac32L_{-1}^2\right)|\chi_2\rangle
\quad\text{is null at }d=26.}
$$

It is spurious, so physicality also proves orthogonality and zero norm without an extra positivity assumption.

**The printed coefficient $3/4$ does not give this [null string state](../../../../../null-string-state.md).** It instead gives $L_1|v_{3/4}\rangle=\tfrac32L_{-1}|\chi_2\rangle$, generally nonzero. For a normalized highest-weight parent with weight $-1$ at $d=26$, the descendant [Gram matrix](../../../../../gram-matrix.md) is

$$
\begin{pmatrix}
\langle L_{-2}\chi_2|L_{-2}\chi_2\rangle&
\langle L_{-2}\chi_2|L_{-1}^2\chi_2\rangle\\
\langle L_{-1}^2\chi_2|L_{-2}\chi_2\rangle&
\langle L_{-1}^2\chi_2|L_{-1}^2\chi_2\rangle
\end{pmatrix}
=\begin{pmatrix}9&-6\\-6&4\end{pmatrix}.
$$

Thus the printed vector has norm $9/4$, whereas the corrected vector has norm zero. This is a genuine PDF coefficient error. Away from 26 dimensions even the corrected coefficient does not give the claimed physical [null string state](../../../../../null-string-state.md); the remaining condition is $L_2|v_{3/2}\rangle=(d-26)|\chi_2\rangle/2$.

The level-two [open string](../../../../../open-string.md) state also needs a source correction: its vector [string oscillator](../../../../../string-oscillator.md) must be $\alpha_{-2}^\mu$, not the printed $\alpha_{-1}^\mu$. A single $\alpha_{-1}$ has level one and cannot share the stated [mass-shell condition](../../../../../string-mass-shell-condition.md) with the two-$\alpha_{-1}$ term. Put $q^\mu=\alpha_0^\mu=\sqrt{2\alpha'}p^\mu$, and write the genuine level-two state as

$$
|\phi\rangle=
\left(a_{\mu\nu}\alpha_{-1}^\mu\alpha_{-1}^\nu+
b_\mu\alpha_{-2}^\mu\right)|p\rangle,
\qquad a_{\mu\nu}=a_{\nu\mu}.
$$

The [mass-shell condition](../../../../../string-mass-shell-condition.md) $L_0=1$ gives $\alpha'p^2+2=1$, so $q^2=-2$. The commutators above give

$$
L_1|\phi\rangle=2(q^\mu a_{\mu\nu}+b_\nu)\alpha_{-1}^\nu|p\rangle,
\qquad
L_2|\phi\rangle=(a^\mu{}_{\mu}+2q\cdot b)|p\rangle.
$$

For the second formula, the contraction from the two $\alpha_{-1}$ operators is exactly $a^\mu{}_{\mu}$, not twice that value. Modes $m>2$ vanish automatically. We have derived

$$
\boxed{b_\nu=-q^\mu a_{\mu\nu},\qquad
 t:=a^\mu{}_{\mu}=-2q\cdot b.}
$$

The coefficient formulas in the question are consequently consistent after the [string oscillator](../../../../../string-oscillator.md) correction and with $d=26$.

To prove the full [level-two open-string polarization decomposition](../../../../../level-two-open-string-polarization-decomposition.md), not merely check one candidate, define

$$
A_\mu=\frac12\left(b_\mu-\frac t4q_\mu\right),\qquad
c_{\mu\nu}=a_{\mu\nu}-\frac t{20}(3q_\mu q_\nu+\eta_{\mu\nu})
-q_\mu A_\nu-q_\nu A_\mu.
$$

The constraints give $q\cdot b=-t/2$ and therefore $q\cdot A=0$. Contracting $c$ with $q$ gives

$$
q^\mu c_{\mu\nu}=-b_\nu+\frac t4q_\nu+2A_\nu=0.
$$

Its trace is $t-t(26+3q^2)/20-2q\cdot A=0$. Thus $c$ is symmetric, traceless and transverse. Conversely, arbitrary $t$, a vector $A$ with $q\cdot A=0$, and such a tensor $c$ give

$$
\boxed{a_{\mu\nu}=\frac t{20}(3q_\mu q_\nu+\eta_{\mu\nu})
+q_\mu A_\nu+q_\nu A_\mu+c_{\mu\nu},\qquad
b_\mu=\frac t4q_\mu+2A_\mu,}
$$

and direct contraction verifies both constraints. The number $20$ uses $d=26$; it would not reproduce the same unrestricted trace in arbitrary dimension.

Finally the two unphysical pieces are precisely the descendants already proved null. The vector part is

$$
|n_1\rangle=L_{-1}\left(2A\cdot\alpha_{-1}|p\rangle\right),
$$

whose parent has $L_0=0$ and all positive modes zero because $q\cdot A=0$. For the scalar part use

$$
L_{-2}|p\rangle=\left(q\cdot\alpha_{-2}+\frac12\alpha_{-1}\cdot\alpha_{-1}\right)|p\rangle,
\quad
L_{-1}^2|p\rangle=\left((q\cdot\alpha_{-1})^2+q\cdot\alpha_{-2}\right)|p\rangle.
$$

Then

$$
|n_2\rangle=\frac t{10}\left(L_{-2}+\frac32L_{-1}^2\right)|p\rangle
$$

has exactly the scalar tensor $t(3q_\mu q_\nu+\eta_{\mu\nu})/20$ and vector $tq_\mu/4$. The momentum vacuum has $L_0=-1$ and positive modes zero, as required. Hence

$$
\boxed{|\phi\rangle=c_{\mu\nu}\alpha_{-1}^\mu\alpha_{-1}^\nu|p\rangle+|n_1\rangle+|n_2\rangle.}
$$

The physical quotient contains only the transverse traceless tensor. Its massive little-group space has dimension $25\cdot26/2-1=324$, agreeing with the [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md) count $24\cdot25/2+24=324$ at level two.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
