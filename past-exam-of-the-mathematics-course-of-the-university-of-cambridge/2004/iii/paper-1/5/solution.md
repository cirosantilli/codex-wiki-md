<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Specify a commutative ground [ring](../../../../../ring.md) $k$ and a unital associative $k$-[algebra](../../../../../algebra-split.md) $R$. For an $R$-[bimodule](../../../../../bimodule.md) $M$, the [Hochschild cochain complex](../../../../../hochschild-cochain-complex.md) has

$$
C^q(R,M)=\operatorname{Hom}_k(R^{\otimes_kq},M),\qquad C^0(R,M)=M,
$$

and coboundary

$$
\begin{aligned}
(\delta f)(a_1,\ldots,a_{q+1})={}&a_1f(a_2,\ldots,a_{q+1})\\
&+\sum_{i=1}^{q}(-1)^if(a_1,\ldots,a_ia_{i+1},\ldots,a_{q+1})\\
&+(-1)^{q+1}f(a_1,\ldots,a_q)a_{q+1}.
\end{aligned}
$$

The [bimodule](../../../../../bimodule.md) identities and [associativity](../../../../../associative-property.md) cancel the terms of $\delta^2$ in pairs. The [Hochschild cohomology](../../../../../hochschild-cohomology.md) is $HH_k^q(R,M)=\ker\delta_q/\operatorname{im}\delta_{q-1}$; the paper's $H^q(R,R)$ uses the regular [bimodule](../../../../../bimodule.md) as coefficients.

Over a [field](../../../../../field.md), the [bar resolution of an associative algebra](../../../../../bar-resolution-of-an-associative-algebra.md) explains its homological meaning. Put $R^e=R\otimes_kR^{\mathrm{op}}$. The degree-$q$ bar term is $R^{\otimes_k(q+2)}$, with the outer factors supplying the $R^e$ action, boundary obtained by multiplying adjacent factors with alternating signs, and augmentation multiplication $R\otimes R\to R$. Inserting $1$ at the left gives a $k$-linear contracting homotopy, proving exactness. The terms are free $R^e$-[modules](../../../../../module-mathematics.md) after choosing a $k$-basis for the inner tensor factors. Applying $\operatorname{Hom}_{R^e}(-,M)$ gives precisely the displayed cochain complex and therefore

$$
HH_k^q(R,M)\cong\operatorname{Ext}_{R^e}^q(R,M).
$$

This [ground-ring qualification in Hochschild cohomology](../../../../../ground-ring-qualification-in-hochschild-cohomology.md) matters for an arbitrary [ring](../../../../../ring.md): one can take $k=\mathbb Z$, but the bar terms need not be projective over $R^e$. The ordinary cochain complex then computes relative [Hochschild cohomology](../../../../../hochschild-cohomology.md); the absolute Ext identification needs, for example, $R$ projective over $k$. Likewise the extension classification below applies to ground-ring-linearly split extensions. For algebras over a [field](../../../../../field.md) these qualifications are automatic.

In degree zero, $(\delta m)(a)=am-ma$, so **$HH^0(R,R)=Z(R)$**. In degree one the cocycle equation is

$$
a\,d(b)-d(ab)+d(a)b=0,
$$

exactly the Leibniz rule for a [derivation of an algebra](../../../../../derivation-of-an-algebra.md). The coboundaries are the [inner derivations](../../../../../inner-derivation.md) $a\mapsto am-ma$. Thus the [First Hochschild cohomology as outer derivations](../../../../../first-hochschild-cohomology-as-outer-derivations.md) is

$$
\boxed{HH^1(R,R)=\operatorname{Der}_k(R)/\operatorname{Inn}(R).}
$$

Its significance is infinitesimal [automorphisms](../../../../../automorphism.md) modulo inner ones. Over the [dual numbers](../../../../../dual-number.md) $k[\varepsilon]/(\varepsilon^2)$, the map $a\mapsto a+\varepsilon d(a)$ is multiplicative precisely when $d$ satisfies the Leibniz rule. Conjugation by $1+\varepsilon m$ gives $a\mapsto a+\varepsilon(ma-am)$, an inner [derivation](../../../../../derivation-of-an-algebra.md) with the opposite sign convention. The quotient therefore measures infinitesimal symmetry not arising from conjugation.

Degree two controls extensions and changes of multiplication. A $k$-linear split [square-zero extension of an algebra](../../../../../square-zero-extension-of-an-algebra.md) with prescribed kernel [bimodule](../../../../../bimodule.md) $M$ can be written as $E=R\oplus M$. Choose a unital section and let $f(a,b)$ be the difference between its product and its value on $ab$. Then

$$
(a,u)(b,v)=(ab,av+ub+f(a,b)).
$$

Computing both parenthesizations of a triple gives the [associativity](../../../../../associative-property.md) condition

$$
a f(b,c)-f(ab,c)+f(a,bc)-f(a,b)c=0,
$$

namely $\delta f=0$. A unital product has $f(1,a)=f(a,1)=0$, so one uses the [normalized Hochschild cochain complex](../../../../../normalized-hochschild-cochain-complex.md). Changing section by $g:R\to M$ gives $f\mapsto f+\delta g$. Conversely the displayed product for any normalized two-cocycle constructs such an extension, and a section change gives the corresponding extension isomorphism. This proves that [second Hochschild cohomology classifies split square-zero extensions](../../../../../second-hochschild-cohomology-classifies-split-square-zero-extensions.md):

$$
\boxed{HH^2(R,M)\text{ classifies these extensions, up to equivalence fixing }R,M.}
$$

The zero class is the split algebra extension with no extra product term. With $M=R$, this gives one meaning of the requested $H^2(R,R)$.

For a [first-order associative deformation](../../../../../first-order-associative-deformation.md), retain the underlying $k$-[module](../../../../../module-mathematics.md) and put $a*b=ab+\varepsilon f(a,b)$. Expanding $(a*b)*c=a*(b*c)$ modulo $\varepsilon^2$ gives exactly $\delta f=0$. A coordinate change $T=1+\varepsilon g$ transports the product to $T^{-1}(T(a)*T(b))$, whose first-order coefficient is $f+\delta g$. Hence

$$
\boxed{HH^2(R,R)\text{ is the space of inequivalent first-order changes of multiplication.}}
$$

This classification is of infinitesimal deformations, not a guarantee that all classes extend to every order. For $a*b=ab+tf(a,b)+t^2\mu_2(a,b)$ modulo $t^3$, the next [associativity](../../../../../associative-property.md) equation is

$$
\delta\mu_2(a,b,c)=f(f(a,b),c)-f(a,f(b,c)).
$$

Substitution of $\delta f=0$ shows the right-hand side is a three-cocycle. Its class in $HH^3(R,R)$ is the [second-order obstruction to an associative deformation](../../../../../second-order-obstruction-to-an-associative-deformation.md). It must vanish for a second-order extension to exist. At higher orders the same expansion gives further obstruction cocycles. If $HH^2(R,R)=0$, every first nonzero coefficient of a [formal associative deformation](../../../../../formal-associative-deformation.md) is a coboundary and can be removed by a coordinate change. Repeating this order by order gives [formal rigidity from vanishing second Hochschild cohomology](../../../../../formal-rigidity-from-vanishing-second-hochschild-cohomology.md), with the transformations converging in the $t$-adic topology. Vanishing of $HH^3$ instead removes these extension obstructions; these are distinct roles.

Examples make the two low degrees concrete. For $R=k[x]$ over a [field](../../../../../field.md), [inner derivations](../../../../../inner-derivation.md) vanish and every [derivation](../../../../../derivation-of-an-algebra.md) is $h(x)\partial_x$, determined by its value on $x$. The [bimodule](../../../../../bimodule.md) resolution

$$
0\longrightarrow k[x]\otimes k[x]
\xrightarrow{\,x\otimes1-1\otimes x\,}
 k[x]\otimes k[x]\longrightarrow k[x]\longrightarrow0
$$

is exact: the middle tensor [ring](../../../../../ring.md) is the polynomial [integral domain](../../../../../integral-domain.md) $k[u,v]$, multiplication identifies its quotient by $u-v$, and multiplication by $u-v$ is injective. Applying [bimodule](../../../../../bimodule.md) Hom gives zero differential. Consequently the [Hochschild cohomology of a polynomial algebra in one variable](../../../../../hochschild-cohomology-of-a-polynomial-algebra-in-one-variable.md) is

$$
HH^0(k[x])=k[x],\qquad HH^1(k[x])=k[x]\partial_x,\qquad HH^q(k[x])=0\quad(q\ge2).
$$

This algebra has many infinitesimal [automorphisms](../../../../../automorphism.md), while its ordinary associative multiplication is formally rigid.

For $R=k[x,y]$ in characteristic zero, the bilinear map $f(a,b)=(\partial_ya)(\partial_xb)$ is a two-cocycle: substitution in $\delta f$ and the two product rules cancel its four terms. It is not a coboundary, because every $\delta g$ on a commutative [algebra](../../../../../algebra-split.md) is symmetric in its two inputs, whereas $f(y,x)-f(x,y)=1$. This class integrates to the [Weyl deformation of a polynomial algebra in two variables](../../../../../weyl-deformation-of-a-polynomial-algebra-in-two-variables.md), with $yx-xy=t$. The differential [Ore extension](../../../../../ore-extension.md) construction supplies the ordered [basis](../../../../../basis.md) $x^iy^j$ over $k[t]$, so the $t$-adic completion has the fixed underlying [module](../../../../../module-mathematics.md) $k[x,y][[t]]$. Its first multiplication correction is exactly this $f$. This displays a genuinely noncommutative [formal associative deformation](../../../../../formal-associative-deformation.md) detected by $HH^2$.

Finally, the [Hochschild cup product](../../../../../hochschild-cup-product.md) $(f\smile g)(a_1,\ldots,a_{p+q})=f(a_1,\ldots,a_p)g(a_{p+1},\ldots,a_{p+q})$ descends to the graded cohomology algebra, and the [Gerstenhaber bracket](../../../../../gerstenhaber-bracket.md) organizes the interaction of [derivations](../../../../../derivation-of-an-algebra.md) and [formal associative deformation](../../../../../formal-associative-deformation.md) cocycles. The calculations above explain why the first two positive degrees are especially useful: $HH^1$ measures outer infinitesimal symmetries, while $HH^2$ measures split extensions and infinitesimal associative structures, with degree three detecting the first obstruction to continuing them.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
