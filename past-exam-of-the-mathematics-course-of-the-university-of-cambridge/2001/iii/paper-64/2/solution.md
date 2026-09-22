<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use one bosonic oscillator sector in [old covariant string quantization](../../../../../old-covariant-string-quantization.md), with the usual [normal-ordering constant of a string](../../../../../normal-ordering-constant-of-a-string.md) $a=1$. Its matter [Virasoro algebra](../../../../../virasoro-algebra.md) and Hermiticity convention are

$$
[L_m,L_n]=(m-n)L_{m+n}+\frac d{12}m(m^2-1)\delta_{m+n,0},\qquad L_n^\dagger=L_{-n}.
$$

A [physical string state](../../../../../physical-string-state.md) satisfies $L_{n>0}|\Psi\rangle=0$ and $(L_0-1)|\Psi\rangle=0$. Let $|k\rangle$ be the oscillator vacuum with $L_{n>0}|k\rangle=0$ and $L_0|k\rangle=h|k\rangle$. For a level-two descendant, the zero-mode condition gives $h+2=1$, hence $h=-1$. The vacuum carrying this momentum is not itself a physical level-zero tachyon state; its descendant is the candidate physical state. With open-string normalization $h=\alpha'k^2$, the required momentum has $k^2=-1/\alpha'$.

The positive-mode conditions can be computed without assuming the answer. First,

$$
L_1L_{-2}|k\rangle=3L_{-1}|k\rangle,\qquad
L_1L_{-1}^2|k\rangle=(4h+2)L_{-1}|k\rangle.
$$

The latter follows by expanding $[L_1,L_{-1}^2]=2L_0L_{-1}+2L_{-1}L_0$ and commuting $L_0$ to the right. Therefore $L_1(L_{-2}+\mu L_{-1}^2)|k\rangle=0$ gives $3-2\mu=0$, or $\mu=3/2$. Similarly,

$$
L_2L_{-2}|k\rangle=(4h+d/2)|k\rangle,\qquad
L_2L_{-1}^2|k\rangle=6h|k\rangle.
$$

At $h=-1$ and $\mu=3/2$ the second condition is $(d/2-13)|k\rangle=0$. Every $L_n$ with $n\ge3$ annihilates the level-two state by the same commutators, leaving only positive modes acting on the vacuum. Thus

$$
\boxed{|Z\rangle=(L_{-2}+\tfrac32L_{-1}^2)|k\rangle\text{ is physical at }d=26.}
$$

This is the [level-two scalar Virasoro null state](../../../../../level-two-scalar-virasoro-null-state.md).

For the norm, take the vacuum norm to be one, suppressing the continuum momentum delta function. The [level-two Virasoro descendant Gram matrix](../../../../../level-two-virasoro-descendant-gram-matrix.md) is

$$
G_2=\begin{pmatrix}4h+d/2&6h\\6h&4h(2h+1)\end{pmatrix}.
$$

The entries follow from $\langle k|L_2L_{-2}|k\rangle$, $\langle k|L_2L_{-1}^2|k\rangle$ and $\langle k|L_1^2L_{-1}^2|k\rangle$, respectively. At $h=-1$,

$$
\langle Z|Z\rangle=(d/2-4)+2(3/2)(-6)+(3/2)^2(4)=\frac{d-26}{2}.
$$

Consequently **the physical state at $d=26$ has norm squared zero**. It is a [spurious string state](../../../../../spurious-string-state.md) as well as physical: for any physical $|\Phi\rangle$, $\langle\Phi|Z\rangle=\langle L_2\Phi|k\rangle+\tfrac32\langle L_1^2\Phi|k\rangle=0$. The [null-state quotient of a string](../../../../../null-state-quotient-of-a-string.md) therefore identifies it with zero. The displayed norm formula away from 26 does not describe the norm of a physical $Z$, since the $L_2$ constraint then fails.

The full covariant [Fock space](../../../../../fock-space.md) is indefinite because timelike [string oscillators](../../../../../string-oscillator.md) have negative norm. The [no-ghost theorem for the critical bosonic string](../../../../../no-ghost-theorem-for-the-critical-bosonic-string.md) states that the constraints at $d=26,a=1$ make the physical inner product positive semidefinite. Every physical state can be represented by a positive transverse state plus a physical null state. Modding out the latter leaves a positive physical space, rather than retaining negative-norm states and simply ignoring them.

One outline of the proof uses [DDF operators](../../../../../ddf-operator.md). Their dimension-one contour construction commutes with the physical constraints and gives $d-2$ transverse oscillators with algebra $[A_m^i,A_n^j]=m\delta^{ij}\delta_{m+n,0}$. Their oscillator states have manifestly positive norm. The covariant constraints and spurious descendants can be organized triangularly in the remaining timelike and longitudinal oscillators. At the critical dimension the completeness step shows that their remaining physical contribution is null, so the 24 transverse DDF oscillators represent the whole quotient.

For integer $2\le d<26$ at the same intercept $a=1$, the [no-ghost theorem below the critical bosonic dimension](../../../../../no-ghost-theorem-below-the-critical-bosonic-dimension.md) gives nonnegative physical norm as well. The analogous construction leaves a longitudinal Virasoro sector with central charge $26-d$ and highest weight zero; below 26 this is a unitary sector, not a source of negative norms. At 26 it becomes null. Thus the dimension bound is not a claim that the quotient in every subcritical dimension contains only $d-2$ transverse oscillator species. The argument assumes the ordinary nonzero-momentum sector where the reference null direction for the DDF construction can be chosen. It does not eliminate the bosonic [tachyon](../../../../../tachyon.md), whose negative mass squared differs from a negative norm, nor the auxiliary [Faddeev-Popov ghosts](../../../../../faddeev-popov-ghost.md). Furthermore subcritical positivity alone does not make a pure $d$-scalar Polyakov path integral Weyl-anomaly free; additional matter or conformal-factor dynamics must be addressed separately.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
