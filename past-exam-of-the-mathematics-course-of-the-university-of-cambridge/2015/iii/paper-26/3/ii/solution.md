<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Logarithms on sufficiently deep units.** Suppose $\operatorname{char}K=0$, let $\ell$ be the [residue characteristic](../../../../../../residue-characteristic.md), and put $e=v(\ell)$. For every integer $r>e/(\ell-1)$ the [p-adic logarithm](../../../../../../p-adic-logarithm.md) and [p-adic exponential function](../../../../../../p-adic-exponential-function.md), evaluated in $K$, converge on the required domains:

$$
\log(1+x)=\sum_{m\geq1}\frac{(-1)^{m+1}x^m}{m},\qquad
\exp(y)=\sum_{m\geq0}\frac{y^m}{m!}.
$$

The bounds $v(m!)=e\,v_\ell(m!)\leq e(m-1)/(\ell-1)$ and $v(m)\leq e(m-1)/(\ell-1)$ show that, for $x,y\in\pi^r\mathcal O_K$, every term beyond the linear one has [valuation](../../../../../../valuation.md) strictly greater than $v(x)$ or $v(y)$. The series therefore converge and preserve these lattices; in particular $\exp(y)\in1+\pi^r\mathcal O_K$. Their formal composition and addition identities are valid by convergence, giving inverse continuous group homomorphisms

$$
\log:1+\pi^r\mathcal O_K\xrightarrow{\;\cong\;}\pi^r\mathcal O_K,
\qquad \exp:\pi^r\mathcal O_K\xrightarrow{\;\cong\;}1+\pi^r\mathcal O_K.
$$

Thus the [logarithm isomorphism on deep principal units](../../../../../../logarithm-isomorphism-on-deep-principal-units.md) is

$$
\boxed{1+\pi^r\mathcal O_K\cong(\mathcal O_K,+),
\qquad u\longmapsto\pi^{-r}\log u,\quad r>\frac e{\ell-1}.}
$$

The right-hand group is torsion-free.

**Roots of unity in $\mathbb Q_p$.** For odd $p$, take $\ell=p,e=1,r=1$. The [principal unit](../../../../../../principal-unit.md) group $1+p\mathbb Z_p$ is torsion-free by the [logarithm isomorphism on deep principal units](../../../../../../logarithm-isomorphism-on-deep-principal-units.md). The [Teichmuller representative](../../../../../../teichmuller-representative.md) splitting leaves precisely the $p-1$ roots in $\mu_{p-1}$.

For $p=2$, take $r=2$. Each odd unit is uniquely $\pm u$ with $u\in1+4\mathbb Z_2$, since its residue modulo four is either one or minus one. This latter group is torsion-free. Consequently

$$
\boxed{|\mu(\mathbb Q_p)|=
\begin{cases}p-1,&p\text{ odd},\\2,&p=2,\end{cases}
\qquad \mu(\mathbb Q_2)=\{1,-1\}.}
$$

This computes the [roots of unity in the p-adic numbers](../../../../../../roots-of-unity-in-the-p-adic-numbers.md).

**The units of $\mathbb Q_2(i)$.** Set $\pi=1-i$. Its polynomial $T^2-2T+2$ is [Eisenstein](../../../../../../eisenstein-criterion.md), so

$$
\mathcal O_K=\mathbb Z_2[i],\qquad v(\pi)=1,\quad v(2)=2,\quad k=\mathbb F_2.
$$

The [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md) facts justifying this are stated in the next solution. Write $U_s=1+\pi^s\mathcal O_K$. Reduction gives $\mathcal O_K^\times=U_1$, and the [successive quotients of principal-unit groups](../../../../../../successive-quotients-of-principal-unit-groups.md)

$$
U_s/U_{s+1}\cong(k,+),\qquad
1+\pi^s b\longmapsto\bar b
$$

have order two for $s\geq1$. Hence $[U_1:U_3]=4$. The four roots in $\mu_4=\{1,i,-1,-i\}$ have distinct images modulo $U_3$, since

$$
v(i-1)=v(-i-1)=1,\qquad v(-1-1)=2.
$$

They exhaust the quotient and intersect $U_3$ trivially. Since $r=3>2/(2-1)$, the [logarithm isomorphism on deep principal units](../../../../../../logarithm-isomorphism-on-deep-principal-units.md) gives $U_3\cong(\mathcal O_K,+)$. Therefore the [unit decomposition of the 2-adic Gaussian field](../../../../../../unit-decomposition-of-the-2-adic-gaussian-field.md) is

$$
\boxed{\mathcal O_K^\times=\mu_4\times U_3
\cong\mu_4\times(\mathcal O_K,+).}
$$

In particular these four elements are all its roots of unity.

**[Quadratic extensions](../../../../../../quadratic-extension.md).** A nonzero element of $K$ is uniquely a power of $\pi$ times a unit, so $K^\times\cong\pi^{\mathbb Z}\times\mathcal O_K^\times$. Squaring on the decomposition above acts as squaring on $\mu_4$ and multiplication by two on the additive ring $\mathcal O_K=\mathbb Z_2\oplus\mathbb Z_2i$. Thus the [square-class group of the 2-adic Gaussian field](../../../../../../square-class-group-of-the-2-adic-gaussian-field.md) is

$$
\boxed{K^\times/(K^\times)^2
\cong C_2\times(\mu_4/\mu_4^2)\times(\mathcal O_K/2\mathcal O_K)
\cong C_2^4.}
$$

By [quadratic extensions from square classes](../../../../../../quadratic-extensions-from-square-classes.md), in characteristic different from two the nontrivial [square classes](../../../../../../square-class.md) classify [quadratic extensions](../../../../../../quadratic-extension.md) $K(\sqrt a)$: two such extensions are $K$-isomorphic exactly when $a/b$ is a square. There are therefore $\boxed{2^4-1=15}$ [quadratic extensions](../../../../../../quadratic-extension.md) up to $K$-isomorphism.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
