<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [old covariant quantization](../../../../../old-covariant-string-quantization.md) of a free-ended bosonic string retains oscillators in all target directions. In mostly-plus [Minkowski spacetime](../../../../../minkowski-spacetime.md), set $\alpha_0^m=\sqrt{2\alpha'}p^m$ and

$$
[\alpha_k^m,\alpha_l^n]=k\,\eta^{mn}\delta_{k+l,0},\qquad
L_n=\frac12\sum_k:\alpha_{n-k}\cdot\alpha_k:,\qquad
L_0=\alpha'p^2+N.
$$

Time-coordinate excitations have negative norms in this covariant [Fock space](../../../../../fock-space.md). The [string ghost states](../../../../../negative-norm-string-state.md) in this discussion are unwanted negative-norm physical states, distinct from the anticommuting [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md) in the [path integral](../../../../../path-integral.md). Constraints and the [null-state quotient of a string](../../../../../null-state-quotient-of-a-string.md) remove unphysical polarizations while maintaining target-space [Lorentz covariance](../../../../../lorentz-covariance.md).

**Why only positive-mode constraints annihilate states.** The quantum [Virasoro algebra](../../../../../virasoro-algebra.md) is

$$
[L_m,L_n]=(m-n)L_{m+n}+\frac D{12}m(m^2-1)\delta_{m+n,0}.
$$

The physical conditions are

$$
\boxed{(L_0-a)|\psi\rangle=0,\qquad L_n|\psi\rangle=0\quad(n>0),}
$$

where $a$ is the [string intercept](../../../../../normal-ordering-constant-of-a-string.md). If both positive and negative modes annihilated states, $[L_1,L_{-1}]=2L_0$ would force $a=0$. Then $[L_2,L_{-2}]=4L_0+D/2$ would force $D=0$. Thus the [Virasoro central extension](../../../../../virasoro-central-extension.md) and shifted zero mode prevent imposing every classical constraint strongly in a nontrivial string. As in [Gupta-Bleuler quantization](../../../../../gupta-bleuler-formalism.md), negative-mode conditions act on physical bras, rather than also annihilating physical kets. Physical [null string states](../../../../../null-string-state.md) are quotiented because their inner products with all physical states vanish.

**The intercept bound at level one.** For $|\epsilon;p\rangle=\epsilon_m\alpha_{-1}^m|p\rangle$, the constraints and norm are

$$
p\cdot\epsilon=0,\qquad p^2=\frac{a-1}{\alpha'},\qquad
\langle\epsilon;p|\epsilon;p\rangle=\epsilon^*\cdot\epsilon.
$$

If $a>1$, momentum is spacelike and its orthogonal complement contains a timelike negative-norm polarization. The [level-one intercept bound in covariant string quantization](../../../../../level-one-intercept-bound-in-covariant-string-quantization.md) is therefore

$$
\boxed{a\leq1.}
$$

For $a<1$, momentum is timelike and the $D-1$ orthogonal polarizations are positive. This avoids level-one ghosts but gives a [massive vector](../../../../../massive-vector-particle.md) with one more polarization than the transverse [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md) spectrum. Ghost absence alone is weaker than equivalence.

For $a=1$, momentum is null. Its orthogonal complement contains $D-2$ positive directions and the null direction $p$. The state $p\cdot\alpha_{-1}|p\rangle$, proportional to $L_{-1}|p\rangle$, is physical, spurious and null. Removing it gives

$$
\boxed{\epsilon\sim\epsilon+\lambda p.}
$$

The quotient has exactly the $D-2$ massless transverse vector polarizations. Thus **equivalence at level one selects $a=1$ and the [null-state quotient of a string](../../../../../null-state-quotient-of-a-string.md)**, not just the inequality.

**Level two and the dimension.** Set $a=1$. At level two, $p^2=-1/\alpha'$ and $k=\sqrt{2\alpha'}p$ has $k^2=-2$. A general state is

$$
|\psi\rangle=\left(\frac12\epsilon_{mn}\alpha_{-1}^m\alpha_{-1}^n
+\zeta_m\alpha_{-2}^m\right)|p\rangle,\qquad\epsilon_{mn}=\epsilon_{nm}.
$$

Using $[L_m,\alpha_n^a]=-n\alpha_{m+n}^a$, the nontrivial positive-mode conditions are

$$
k^m\epsilon_{mn}+2\zeta_n=0,\qquad
\epsilon^m{}_m+4k\cdot\zeta=0.
$$

There are $D-1$ vector [null string states](../../../../../null-string-state.md) $L_{-1}(v\cdot\alpha_{-1}|p\rangle)$ with $k\cdot v=0$. The parent has $L_0=0$, so the descendant norm is zero. Quotienting these leaves the massive [symmetric traceless rank-two tensor](../../../../../symmetric-trace-free-square-of-the-defining-orthogonal-representation.md) plus one additional scalar.

The [level-two scalar in covariant string quantization](../../../../../level-two-scalar-in-covariant-string-quantization.md) can be chosen, for every $D$, as

$$
|S_D\rangle=\left[\alpha_{-1}\cdot\alpha_{-1}
+\frac{D+4}{10}(k\cdot\alpha_{-1})^2
+\frac{D-1}{5}k\cdot\alpha_{-2}\right]|p\rangle.
$$

On its three displayed structures, $L_1$ gives respectively $2,-4,2$ times $k\cdot\alpha_{-1}|p\rangle$, and $L_2$ gives $D,-2,-4$ times the vacuum. The coefficients make both combinations vanish. The first two structures have norms $2D,8$ and cross inner product $-4$; the mode-two structure has norm $-4$ and is orthogonal to them. For $B=(D+4)/10$, $C=(D-1)/5$, this yields

$$
\boxed{\langle S_D|S_D\rangle
=2D-8B+8B^2-4C^2
=\frac{2}{25}(D-1)(26-D).}
$$

Above 26 this is a physical [negative-norm string state](../../../../../negative-norm-string-state.md). Below 26 it is an extra positive-norm scalar, which cannot be discarded just to force the ordinary light-cone state count. At 26 it becomes null and can be removed. Thus level-two ghost absence gives $D\leq26$, whereas **equivalence to the ordinary transverse spectrum requires $D=26$**.

The critical scalar is also a [Virasoro descendant](../../../../../virasoro-descendant.md). For $L_0|p\rangle=-|p\rangle$, the [level-two scalar Virasoro null state](../../../../../level-two-scalar-virasoro-null-state.md) candidate

$$
|Z\rangle=\left(L_{-2}+\frac32L_{-1}^2\right)|p\rangle
$$

obeys

$$
L_1|Z\rangle=0,\qquad L_2|Z\rangle=\frac{D-26}{2}|p\rangle.
$$

At $D=26$ it is physical and null, with $|S_{26}\rangle=2|Z\rangle$. At other dimensions it is not physical, so its norm must not be treated as a physical ghost test; the already-physical $|S_D\rangle$ gives the correct test.

Finally, the covariant level-two oscillator space has dimension $D(D+3)/2$. The $D$ conditions from $L_1$ and one from $L_2$ leave $(D-1)(D+2)/2$ physical components. Quotienting $D-1$ vector null states and the critical scalar null state leaves

$$
\boxed{\frac{D(D-1)}2-1=\frac{(D-2)(D+1)}2,}
$$

the [massive spin-two field](../../../../../massive-spin-two-field.md) count and the level-two [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md) count. The vector null descendants change the components of $\zeta$ orthogonal to $k$, and the critical scalar null descendant changes its component along $k$. Thus $\zeta$ can be set to zero. A representative then has $\zeta=0$, $k^m\epsilon_{mn}=0$ and $\epsilon^m{}_m=0$. The two approaches consequently agree on the massless level-one vector and massive level-two spin-two tensor for $a=1,D=26$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
