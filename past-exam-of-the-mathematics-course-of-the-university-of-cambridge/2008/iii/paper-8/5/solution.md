<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [Hopf algebra](../../../../../hopf-algebra.md) over $k$ is a unital associative algebra $H$ equipped with a [coalgebra](../../../../../coalgebra.md) structure $(\Delta,\varepsilon)$ such that both maps are algebra homomorphisms, and with an [antipode](../../../../../antipode.md) $S:H\to H$. The defining identities are

$$
(\Delta\otimes1)\Delta=(1\otimes\Delta)\Delta,\qquad
(\varepsilon\otimes1)\Delta=1=(1\otimes\varepsilon)\Delta,
$$



$$
m(S\otimes1)\Delta=\eta\varepsilon=m(1\otimes S)\Delta,
$$

where $m$ is multiplication and $\eta:k\to H$ is the unit map; the counit identities use the standard identifications with $k\otimes H$ and $H\otimes k$. The first compatibility conditions define a [bialgebra](../../../../../bialgebra.md); the [antipode](../../../../../antipode.md) provides its convolution inverse. Multiplication commutativity and coproduct cocommutativity are independent conditions, as the two examples below demonstrate.

For the final construction, let $q\in\mathbb C^\times$, with $q\ne\pm1$, and take the numerical [Yang-Baxter R-matrix](../../../../../yang-baxter-r-matrix.md), in the ordered basis $11,12,21,22$,

$$
R=\begin{pmatrix}q&0&0&0\\0&1&0&0\\0&q-q^{-1}&1&0\\0&0&0&q\end{pmatrix}.
$$

It is invertible. Its four action rules are $11\mapsto q11$, $12\mapsto12+(q-q^{-1})21$, $21\mapsto21$, $22\mapsto q22$. Applying these rules on the eight basis vectors of $V^{\otimes3}$ verifies $R_{12}R_{13}R_{23}=R_{23}R_{13}R_{12}$, the [Yang-Baxter equation](../../../../../yang-baxter-equation.md).

In the [RTT construction](../../../../../rtt-construction.md), introduce $T=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$ and impose $RT_1T_2=T_2T_1R$, where $T_1=T\otimes I$, $T_2=I\otimes T$. Entrywise multiplication gives

$$
ab=qba,\quad ac=qca,\quad bd=qdb,\quad cd=qdc,\quad bc=cb,\quad
ad-da=(q-q^{-1})bc.
$$

For example its $(1,2)$ entry gives $qab=ba+(q-q^{-1})ab$, hence $ab=qba$. Define

$$
\Delta(t_{ij})=\sum_kt_{ik}\otimes t_{kj},\qquad
\varepsilon(t_{ij})=\delta_{ij}.
$$

These maps descend to the RTT algebra. Indeed two matrices $T',T''$ in commuting tensor factors each satisfy RTT, and

$$
R(T'T'')_1(T'T'')_2
=RT'_1T'_2T''_1T''_2
=T'_2T'_1T''_2T''_1R
=(T'T'')_2(T'T'')_1R.
$$

Matrix associativity gives coassociativity and the identity matrix gives the counit. Thus RTT first gives a [bialgebra](../../../../../bialgebra.md); the [R-matrix](../../../../../yang-baxter-r-matrix.md) alone does not automatically provide an [antipode](../../../../../antipode.md).

Here the [quantum determinant](../../../../../quantum-determinant.md) $D=ad-qbc$ is central and satisfies $\Delta D=D\otimes D$, $\varepsilon D=1$, as follows by substitution of the displayed relations. Impose $D=1$. This quotient is the [coordinate Hopf algebra of quantum SL2](../../../../../coordinate-hopf-algebra-of-quantum-sl2.md), with

$$
\boxed{S(T)=\begin{pmatrix}d&-q^{-1}b\\-qc&a\end{pmatrix}.}
$$

These assignments extend as an anti-algebra map: for example reversing $ab-qba$ gives $-q^{-1}bd+db=0$, and reversing the determinant relation gives $ad-qcb=1$. The remaining relations are checked in the same way. Direct multiplication gives $TS(T)=S(T)T=I$: the first diagonal entry of $TS(T)$ is $ad-qbc=1$, its second is $da-q^{-1}cb=1$, and the off-diagonal entries vanish by the $q$-commutation relations. These are precisely the [antipode](../../../../../antipode.md) identities on generators, proving that the quotient is a [Hopf algebra](../../../../../hopf-algebra.md).

To verify both required failures of symmetry, map this algebra onto the [quantum Laurent plane](../../../../../quantum-laurent-plane.md) with generators $u,u^{-1},v$ and relation $uv=qvu$, by $a\mapsto u$, $b\mapsto v$, $c\mapsto0$, $d\mapsto u^{-1}$. Construct this algebra directly on the [vector space](../../../../../vector-space-split.md) with basis $u^iv^j$, $i\in\mathbb Z$, $j\ge0$, and product $(u^iv^j)(u^kv^\ell)=q^{-jk}u^{i+k}v^{j+\ell}$. The exponent identity $-jk-(j+\ell)m=-\ell m-j(k+m)$ makes multiplication associative, and the basis products give $uv=qvu$ with $u$ invertible. Since $uv\ne vu$ for $q\ne1$, the [Hopf algebra](../../../../../hopf-algebra.md) is noncommutative. Under the same quotient in both tensor factors,

$$
\Delta b-\Delta^{\rm op}b\longmapsto
u\otimes v+v\otimes u^{-1}-v\otimes u-u^{-1}\otimes v\ne0,
$$

because the four terms are distinct tensor-basis vectors. Hence it is also noncocommutative. **The construction yields $\boxed{\mathcal O_q(\operatorname{SL}_2)\text{ noncommutative and noncocommutative}}$, for example at $q=2$.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
