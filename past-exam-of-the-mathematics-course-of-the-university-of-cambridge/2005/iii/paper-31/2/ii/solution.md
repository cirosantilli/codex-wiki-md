<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $a,b\in\mathbb Q_p^\times$, the [quadratic Hilbert symbol](../../../../../../quadratic-hilbert-symbol.md) $(a,b)_p$ is one if $b$ is a [field norm](../../../../../../field-norm.md) from $\mathbb Q_p(\sqrt a)$, and minus one otherwise; a square $a$ gives the trivial extension and symbol one. It depends only on the two [square classes](../../../../../../square-class.md). Equivalently, the conic $z^2=ax^2+by^2$ has a nonzero [rational point](../../../../../../rational-point.md) precisely when the symbol is one. Interchanging $a$ and $b$ in the conic gives $(a,b)_p=(b,a)_p$. The [Hilbert norm residue symbol](../../../../../../hilbert-norm-residue-symbol.md) is a [group homomorphism](../../../../../../group-homomorphism.md) in each argument; for nonsquare $a$, the [cyclic local norm index](../../../../../../cyclic-local-norm-index.md) makes its [group kernel](../../../../../../kernel-of-a-group-homomorphism.md) a [subgroup](../../../../../../subgroup.md) of index two. The resulting pairing on [square classes](../../../../../../square-class.md) is nondegenerate. Also

$$
(a,-a)_p=1,\qquad(a,a)_p=(a,-1)_p,
$$

since $N(\sqrt a)=-a$. In the language of [local class field theory](../../../../../../local-class-field-theory.md), $(a,b)_p=\operatorname{Art}_p(b)(\sqrt a)/\sqrt a$; in the [Brauer group](../../../../../../brauer-group.md), it records whether the quaternion [cyclic algebra](../../../../../../cyclic-algebra.md) $(a,b)$ splits. These are compatible norm-obstruction descriptions.

An [unramified extension](../../../../../../unramified-extension.md) of [local fields](../../../../../../local-field.md) of degree two has norm [group](../../../../../../group-split.md) consisting precisely of elements with even [valuation](../../../../../../valuation.md). Indeed,

$$
v_K(Nz)=2v_L(z),
$$

and the norms on units are surjective. For the latter assertion, the norm on the finite [residue fields](../../../../../../residue-field.md) is surjective. On successive [higher principal-unit groups](../../../../../../higher-principal-unit-group.md), the congruence

$$
N(1+\pi^r t)\equiv1+\pi^r\operatorname{Tr}_{\kappa_L/\kappa_K}(\bar t)\pmod{\pi^{r+1}}
$$

allows one to correct a proposed unit norm one digit at a time: the residue [field trace](../../../../../../field-trace.md) is surjective, and [completeness](../../../../../../completeness.md) makes the corrections converge. An unramified quadratic field is unique up to [isomorphism](../../../../../../isomorphism.md). Therefore, if $d$ is its defining nonsquare class,

$$
\boxed{(d,b)_p=(-1)^{v_p(b)}.}
$$

For odd $p$, choose the nonsquare unit $u_0$ from part (i). The [polynomial](../../../../../../polynomial-split.md) $T^2-u_0$ has irreducible separable reduction, so it defines the unramified [quadratic extension](../../../../../../quadratic-extension.md). Thus

$$
\Delta_1=\{1,u_0\},\qquad\Delta_2=\{1,u_0\}.
$$

The trivial class is included in $\Delta_2$, since a degree-one extension is unramified. The two units pair trivially, while $(u_0,p)_p=-1$. Any class outside $\Delta_1$ has odd [valuation](../../../../../../valuation.md) and consequently pairs nontrivially with $u_0$. This proves directly

$$
\boxed{\Delta_1^\perp=\Delta_2,\qquad\Delta_2^\perp=\Delta_1\quad(p\ne2).}
$$

For $p=2$, the unit [square classes](../../../../../../square-class.md) from part (i) give $\Delta_1=\{1,-1,5,-5\}$. The element $\omega=(1+\sqrt5)/2$ satisfies $T^2-T-1$; its reduction $T^2+T+1$ is irreducible and separable over $\mathbb F_2$. This shows that $\mathbb Q_2(\sqrt5)$ is unramified of degree two, giving

$$
\Delta_1=\{1,-1,5,-5\},\qquad\Delta_2=\{1,5\}.
$$

For a fully explicit pairing check, use the generators $(-1,5,2)$. We have $(-1,5)_2=1$ and $(-1,2)_2=1$, since $5=N(1+2i)$ and $2=N(1+i)$ from $\mathbb Q_2(i)$. But $(-1,-1)_2=-1$: a norm equal to $-1$ would be a sum of two squares. If either summand had negative [valuation](../../../../../../valuation.md), the sum would have negative [valuation](../../../../../../valuation.md) (equal negative [valuations](../../../../../../valuation.md) give [valuation](../../../../../../valuation.md) $1-2r<0$); if both were integral, their squares could not sum to $-1\equiv3\pmod4$. Finally, the unramified norm criterion gives $(5,2)_2=-1$. The identity $(a,b)_2=(b,a)_2$ and $(a,a)_2=(a,-1)_2$ determine the remaining entries. Writing $(a,b)_2=(-1)^{B(a,b)}$, the exponent [matrix](../../../../../../matrix.md) is

$$
B=\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix}
\quad\text{in the basis }(-1,5,2).
$$

For $b=(-1)^s5^t2^r$, annihilating both generators $-1,5$ of $\Delta_1$ requires $s=r=0$, so $b\in\{1,5\}$. Annihilating $5$ alone requires $r=0$, so $b$ is a unit class. Hence

$$
\boxed{\Delta_1^\perp=\Delta_2,\qquad\Delta_2^\perp=\Delta_1\quad(p=2).}
$$

These are the [Hilbert-symbol annihilators of units and unramified square classes](../../../../../../hilbert-symbol-annihilators-of-units-and-unramified-square-classes.md). Annihilators here are taken with respect to this pairing, or equivalently in the [character group of a finite abelian group](../../../../../../character-group-of-a-finite-abelian-group.md) after identifying [square classes](../../../../../../square-class.md) with their Hilbert-symbol characters.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
