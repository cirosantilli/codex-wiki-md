# Paper 7

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper7.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper7.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)

## 1

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use $\sigma_A(x)$ and $\rho_A(x)$ for [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) and [algebra resolvent set](../../../banach-algebra.md#resolvent-set-of-a-banach-algebra-element). An inverse in the smaller [unital algebra](../../../associative-algebra.md#unital-algebra) is also an inverse in the larger one, so $\rho_B(x)\subseteq\rho_A(x)$.

If $\lambda\in\rho_B(x)$ and $r=(\lambda1-x)^{-1}\in B$, then for $|\mu-\lambda|\|r\|<1$ the [Neumann series](../../../banach-algebra.md#neumann-series) gives

$$
(\mu1-x)^{-1}=(1+(\mu-\lambda)r)^{-1}r\in B.
$$

Thus $\rho_B(x)$ is [open](../../../topology.md#open-set). To prove relative closedness, suppose $\lambda_n\in\rho_B(x)$ and $\lambda_n\to\lambda\in\rho_A(x)$. [Continuity](../../../calculus.md#continuous-function) of inversion in $A$ gives $(\lambda_n1-x)^{-1}\to(\lambda1-x)^{-1}$. Since $B$ is [norm](../../../functional-analysis.md#norm) [closed](../../../topology.md#closed-set), the limiting inverse belongs to $B$, so $\lambda\in\rho_B(x)$. Consequently **$\rho_B(x)$ is relatively clopen in $\rho_A(x)$**.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

A [connected component](../../../geometry-and-topology.md#connected-component) $U$ of $\rho_A(x)$ meets the relatively clopen subset $\rho_B(x)$ either everywhere or nowhere: its intersection and its complement would otherwise disconnect $U$. If it meets nowhere, $U\subseteq\sigma_B(x)$. If it meets everywhere, $U$ is a [connected](../../../geometry-and-topology.md#connected-space) subset of $\rho_B(x)$, and any larger [connected](../../../geometry-and-topology.md#connected-space) subset of $\rho_B(x)$ would be a [connected](../../../geometry-and-topology.md#connected-space) subset of $\rho_A(x)$ larger than its component $U$. Thus **$U$ is either a whole component of $\rho_B(x)$ or lies wholly in $\sigma_B(x)$**.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For $|\lambda|>\|x\|$, the [Neumann series](../../../banach-algebra.md#neumann-series)

$$
(\lambda1-x)^{-1}=\sum_{n=0}^{\infty}\lambda^{-n-1}x^n
$$

converges in $B$. The exterior of this disk is [connected](../../../geometry-and-topology.md#connected-space) and belongs to both [algebra resolvent sets](../../../banach-algebra.md#resolvent-set-of-a-banach-algebra-element). Since each [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) is [compact](../../../topology.md#compact-space), each [algebra resolvent set](../../../banach-algebra.md#resolvent-set-of-a-banach-algebra-element) has exactly one unbounded component: any unbounded component meets that exterior, and two components meeting a common [connected](../../../geometry-and-topology.md#connected-space) exterior must coincide. Part (ii) says that the component of $\rho_A(x)$ meeting the exterior is also a whole component of $\rho_B(x)$. Hence **the unbounded components are identical**.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Now $B=\overline{\mathbb C[1,x]}$. Let $U$ be a bounded component of $\rho_A(x)$ and $\lambda\in U$. Its [boundary](../../../topology.md#boundary-of-a-set) lies in $\sigma_A(x)$: an [open](../../../topology.md#open-set) disk about a [boundary](../../../topology.md#boundary-of-a-set) point in the [algebra resolvent set](../../../banach-algebra.md#resolvent-set-of-a-banach-algebra-element) would meet $U$ and would belong to the same component, contradicting [boundary](../../../topology.md#boundary-of-a-set) membership. The [maximum modulus principle](../../../complex-analysis.md#maximum-modulus-principle) on the bounded domain $U$ therefore gives, for every complex [polynomial](../../../polynomial.md) $p$,

$$
|p(\lambda)|\le\max_{\partial U}|p|
\le\max_{\sigma_A(x)}|p|=r_A(p(x))\le\|p(x)\|.
$$

Here [spectral mapping theorem](../../../mathematics.md#spectral-mapping-theorem) follows by factoring $p(z)-\mu$: its commuting factors are invertible exactly when every root avoids the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element).

The rule $p(x)\mapsto p(\lambda)$ is well-defined by the displayed bound, multiplicative and bounded on the dense [polynomial](../../../polynomial.md) [subalgebra](../../../algebra.md#subalgebra). It extends to a [unital](../../../associative-algebra.md#unital-algebra) [character](../../../representation-theory.md#character-of-a-representation) $\varphi_\lambda$ on $B$. Since $\varphi_\lambda(\lambda1-x)=0$, that element cannot have an inverse in $B$. Thus **$U\subseteq\sigma_B(x)$**. Together with part (iii), this proves that the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) of a polynomial-generated Banach [subalgebra](../../../algebra.md#subalgebra) is exactly the original [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) with all its bounded complementary components filled in.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

The hypothesis puts zero in the common unbounded resolvent component from part (iii). Hence $0\in\rho_B(x)$ for $B=\overline{\mathbb C[1,x]}$, and $(-x)^{-1}\in B$, or equivalently $x^{-1}\in B$. By the definition of this [norm](../../../functional-analysis.md#norm) [closure](../../../topology.md#closure-topology), for each $n$ choose a [polynomial](../../../polynomial.md) $p_n$ with $\|p_n(x)-x^{-1}\|<1/n$. Therefore

$$
\boxed{p_n(x)\longrightarrow x^{-1}.}
$$

This is an approximation in the algebra [norm](../../../functional-analysis.md#norm), not merely a scalar approximation on the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element).

## 2

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Give $\mathcal O(U)$ the [compact-open topology](../../../real-analysis.md#compact-open-topology). Choose a finite polygonal cycle $\Gamma$ in $U\setminus\sigma_A(x)$ whose [winding number](../../../complex-analysis.md#winding-number) is one on the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) and zero outside $U$. One can take the oriented [boundary](../../../topology.md#boundary-of-a-set) of a finite union of small squares surrounding the [compact](../../../topology.md#compact-space) [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) and contained in $U$. Define

$$
\Theta_x(f)=\frac1{2\pi i}\int_\Gamma f(z)(z1-x)^{-1}\,dz.
$$

The integral is an algebra-norm integral of a [continuous](../../../calculus.md#continuous-function) function on finitely many segments. Cauchy's theorem, applied after any [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) on $A$, makes it independent of the cycle. Moreover

$$
\|\Theta_x(f)\|\le C_\Gamma\sup_{z\in\Gamma}|f(z)|,\qquad
C_\Gamma=\frac{\operatorname{length}(\Gamma)}{2\pi}\max_\Gamma\|(z1-x)^{-1}\|,
$$

so it is [continuous](../../../calculus.md#continuous-function) for the [compact-open topology](../../../real-analysis.md#compact-open-topology).

Here is a direct verification of the algebra properties and uniqueness using the allowed [Runge theorem](../../../complex-analysis.md#runge-s-theorem). The version required is that every [holomorphic function](../../../complex-analysis.md#holomorphic-function) on an [open](../../../topology.md#open-set) plane [set](../../../set.md) is a locally uniform limit of [rational functions](../../../isolated-singularity.md#rational-function) with poles outside that [set](../../../set.md), allowing a [polynomial](../../../polynomial.md) part. A [rational function](../../../isolated-singularity.md#rational-function) $r=p/q$ of this kind has the unambiguous value $r(x)=p(x)q(x)^{-1}$, since the roots of $q$ avoid the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element). These rational values form a [unital algebra](../../../associative-algebra.md#unital-algebra) [homomorphism](../../../algebra.md#homomorphism).

They agree with the [contour integral](../../../complex-analysis.md#contour-integral). First $\frac1{2\pi i}\int_\Gamma(z1-x)^{-1}\,dz=1$, by replacing the cycle with a large circle and integrating its Neumann expansion. The identity $z^j1-x^j=(z1-x)\sum_{k=0}^{j-1}z^{j-1-k}x^k$ then proves the assertion for [polynomials](../../../polynomial.md). For $a\notin U$, the [resolvent identity](../../../banach-algebra.md#resolvent-identity) gives

$$
\frac{(z1-x)^{-1}}{z-a}
=(x-a1)^{-1}\left((z1-x)^{-1}-\frac1{z-a}1\right).
$$

The cycle has [winding number](../../../complex-analysis.md#winding-number) zero at $a$, so integration gives $(x-a1)^{-1}$. This identity holds on a neighborhood of $a$ disjoint from the cycle and the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element). Differentiating with respect to $a$ gives the analogous result for every power $(z-a)^{-k}$, and partial fractions give it for all the [rational functions](../../../isolated-singularity.md#rational-function) under consideration.

If $r_n\to f$ and $s_n\to g$ locally uniformly, the contour estimate makes their evaluated sequences converge. Since $r_ns_n\to fg$ locally uniformly and multiplication in $A$ is [continuous](../../../calculus.md#continuous-function), their limits satisfy $\Theta_x(fg)=\Theta_x(f)\Theta_x(g)$. Also $\Theta_x(1)=1$ and $\Theta_x(Z)=x$. Conversely any [continuous](../../../calculus.md#continuous-function) [unital](../../../associative-algebra.md#unital-algebra) complex-algebra [homomorphism](../../../algebra.md#homomorphism) sending $Z$ to $x$ must send $Z-a$ to $x-a1$ and its reciprocal to the inverse. It therefore agrees on [rational functions](../../../isolated-singularity.md#rational-function) and then, by Runge density and [continuity](../../../calculus.md#continuous-function), on all of $\mathcal O(U)$. This proves **existence and uniqueness of the [holomorphic functional calculus](../../../banach-algebra.md#holomorphic-functional-calculus)**.

For its spectral mapping property, first note compatibility on a smaller [open](../../../topology.md#open-set) spectral neighborhood $W\subseteq U$: composing restriction to $W$ with the calculus there gives the calculus on $U$ by uniqueness. If $\mu\notin g(\sigma_A(x))$, choose such a $W$ where $\mu-g$ never vanishes. Then

$$
(\mu1-\Theta_x(g))^{-1}=\Theta_x\bigl((\mu-g)^{-1}\bigr),
$$

with the right side evaluated on $W$. Conversely, for $\lambda\in\sigma_A(x)$, write $g(z)-g(\lambda)=(z-\lambda)q(z)$ with $q$ [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on $U$. The evaluated factors commute. If their product were invertible, both factors would be invertible, contradicting $\lambda\in\sigma_A(x)$. Thus

$$
\boxed{\sigma_A(\Theta_x(g))=g(\sigma_A(x))\subseteq g(U)\subseteq V.}
$$

Pullback $h\mapsto h\circ g$ is [continuous](../../../calculus.md#continuous-function) from $\mathcal O(V)$ to $\mathcal O(U)$ because the image under $g$ of a [compact](../../../topology.md#compact-space) [set](../../../set.md) is [compact](../../../topology.md#compact-space). The composite $h\mapsto\Theta_x(h\circ g)$ is a [continuous](../../../calculus.md#continuous-function) [unital](../../../associative-algebra.md#unital-algebra) [homomorphism](../../../algebra.md#homomorphism) taking the coordinate function to $y=\Theta_x(g)$. Uniqueness of the calculus at $y$ proves

$$
\boxed{\Theta_y(h)=\Theta_x(h\circ g).}
$$

For the exponential conclusion, let $K=\sigma_A(x)$. There is a simple polygonal arc from zero through its unbounded complementary component to outside a disk containing $K$, continued by a ray to infinity and avoiding $K$. Loops in an initial polygonal path can be removed to make the arc simple. The complement of this slit is a [simply connected](../../../algebraic-topology.md#simply-connected-space) [open](../../../topology.md#open-set) neighborhood of $K$ avoiding zero, and hence admits a [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm) $\ell$. [Set](../../../set.md) $y=\Theta_x(\ell)$. The composition rule gives

$$
\boxed{e^y=\Theta_x(e^\ell)=\Theta_x(Z)=x.}
$$

The calculus of the entire exponential agrees with the usual algebra exponential because its power-series partial sums converge locally uniformly. Finally an invertible [matrix](../../../vector-space.md#matrix) over the [complex numbers](../../../complex-analysis.md#complex-number) has a finite [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) avoiding zero. Removing finitely many plane points leaves a [connected](../../../geometry-and-topology.md#connected-space) [set](../../../set.md), so the hypothesis always holds: **every invertible [matrix](../../../vector-space.md#matrix) over the [complex numbers](../../../complex-analysis.md#complex-number) is an exponential of a [matrix](../../../vector-space.md#matrix) over the [complex numbers](../../../complex-analysis.md#complex-number)**.

## 3

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [C-star algebra](../../../banach-algebra.md#c-star-algebra) is a complex [Banach algebra](../../../banach-algebra.md) with a conjugate-linear involution satisfying $(ab)^*=b^*a^*$ and $\|a^*a\|=\|a\|^2$. The inequality $\|a\|^2\le\|a^*\|\|a\|$, and then the same inequality for $a^*$, show that the involution is [isometric](../../../riemannian-geometry.md#isometry). In a nonzero [unital](../../../associative-algebra.md#unital-algebra) [C-star algebra](../../../banach-algebra.md#c-star-algebra), the identity has [norm](../../../functional-analysis.md#norm) one.

For a [Hermitian algebra element](../../../associative-algebra.md#hermitian-element-of-a-star-algebra) $h$, the exponential $e^{ith}$ is unitary for real $t$ and has [norm](../../../functional-analysis.md#norm) one. If $\lambda\in\sigma(h)$, then $e^{it\lambda}\in\sigma(e^{ith})$: factoring $e^{itz}-e^{it\lambda}=(z-\lambda)q(z)$ with entire $q$ proves this, since the evaluated factors commute. Hence $|e^{it\lambda}|\le1$ for all positive and negative $t$, forcing $\operatorname{Im}\lambda=0$. Thus **[Hermitian algebra elements](../../../associative-algebra.md#hermitian-element-of-a-star-algebra) have real [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element)**.

For a [normal C-star element](../../../banach-algebra.md#normal-element-of-a-c-star-algebra) $a$, commutation of $a,a^*$ gives

$$
\|a^2\|^2=\|(a^*)^2a^2\|=\|(a^*a)^2\|=\|a^*a\|^2=\|a\|^4.
$$

The middle equality of [norms](../../../functional-analysis.md#norm) uses the [C-star identity](../../../banach-algebra.md#c-star-identity) on the [Hermitian algebra element](../../../associative-algebra.md#hermitian-element-of-a-star-algebra) $a^*a$. Iterating along powers $2^n$ and applying the [spectral radius formula](../../../analysis.md#spectral-radius-formula) proves $r(a)=\|a\|$.

Now suppose $A$ is commutative and [unital](../../../associative-algebra.md#unital-algebra). Every [maximal ideal](../../../commutative-algebra.md#maximal-ideal) is [closed](../../../topology.md#closed-set): if it were dense, it would contain an element within distance less than one of the identity, hence an invertible element by the [Neumann series](../../../banach-algebra.md#neumann-series), which is impossible for a proper ideal. Its quotient is a complex Banach division algebra and is therefore $\mathbb C$ by the [Gelfand-Mazur theorem](../../../banach-algebra.md#gelfand-mazur-theorem). [Maximal ideals](../../../commutative-algebra.md#maximal-ideal) thus give [characters](../../../representation-theory.md#character-of-a-representation). Conversely, every [character](../../../representation-theory.md#character-of-a-representation) $\varphi$ satisfies $\varphi(a)\in\sigma_A(a)$, because applying it to an inverse of $a-\varphi(a)1$ would give a contradiction. [Characters](../../../representation-theory.md#character-of-a-representation) are consequently contractive. The converse spectral inclusion follows by placing the proper ideal generated by $a-\lambda1$ in a [maximal ideal](../../../commutative-algebra.md#maximal-ideal). We have proved

$$
\sigma_A(a)=\{\varphi(a):\varphi\in\Phi_A\}.
$$

The [character space](../../../banach-algebra.md#character-space-of-an-algebra) $\Phi_A$ is a weak-star [closed](../../../topology.md#closed-set) subset of the dual unit ball, characterized by $\varphi(1)=1$ and $\varphi(ab)=\varphi(a)\varphi(b)$. The [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) makes it [compact](../../../topology.md#compact-space) Hausdorff. Define the [Gelfand transform](../../../banach-algebra.md#gelfand-representation) by $\widehat a(\varphi)=\varphi(a)$. For Hermitian $h$, its values are real; writing $a=h+ik$ with both terms Hermitian shows $\widehat{a^*}=\overline{\widehat a}$. In the commutative algebra every element is normal, so

$$
\|\widehat a\|_\infty=r(a)=\|a\|.
$$

The transform is therefore an [isometric](../../../riemannian-geometry.md#isometry) [unital](../../../associative-algebra.md#unital-algebra) star-homomorphism and has [closed](../../../topology.md#closed-set) range in $C(\Phi_A)$. Its range separates [characters](../../../representation-theory.md#character-of-a-representation) by their definition and is [closed](../../../topology.md#closed-set) under complex conjugation. The complex [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem) makes that range dense, hence equal to $C(\Phi_A)$. This proves the [Commutative Gelfand--Naimark theorem](../../../banach-algebra.md#commutative-gelfand-naimark-theorem):

$$
\boxed{A\cong C(\Phi_A)\quad\text{isometrically as a star algebra}.}
$$

For a nonunital [C-star algebra](../../../banach-algebra.md#c-star-algebra), its [C-star unitization](../../../banach-algebra.md#unitization-of-a-c-star-algebra) can be constructed without assuming an operator representation on a [Hilbert space](../../../hilbert-space.md). Represent $A$ by left multiplication on itself, which is [isometric](../../../riemannian-geometry.md#isometry) because testing $L_a$ on $a^*/\|a\|$ gives $\|L_a\|=\|a\|$. Adjoin the identity operator and [set](../../../set.md) $\|z\|=\|L_z\|$. For $z=a+\lambda1$ and $b\in A$, the [C-star identity](../../../banach-algebra.md#c-star-identity) in $A$ gives $\|zb\|^2=\|b^*z^*zb\|\le\|b\|\|L_{z^*z}b\|$. Consequently $\|L_z\|^2\le\|L_{z^*z}\|\le\|L_{z^*}\|\|L_z\|$. Applying this also to $z^*$ proves that the new involution is [isometric](../../../riemannian-geometry.md#isometry) and that its [C-star identity](../../../banach-algebra.md#c-star-identity) holds. The extension by the identity is complete, since the [isometric](../../../riemannian-geometry.md#isometry) image of $A$ is [closed](../../../topology.md#closed-set) and one adjoins just one dimension. Apply the [unital](../../../associative-algebra.md#unital-algebra) result to a commutative $A^+$; the [character](../../../representation-theory.md#character-of-a-representation) $\infty$ given by $a+\lambda1\mapsto\lambda$ has kernel $A$. Under the isomorphism, this kernel consists of the [continuous](../../../calculus.md#continuous-function) functions vanishing at $\infty$. Thus **$A\cong C_0(\Phi_A)$** in the nonunital case, with locally [compact](../../../topology.md#compact-space) [character space](../../../banach-algebra.md#character-space-of-an-algebra) $\Phi_A=\Phi_{A^+}\setminus\{\infty\}$.

For a Hermitian $h$ in a possibly noncommutative algebra, apply this result to the commutative [unital](../../../associative-algebra.md#unital-algebra) [C-star subalgebra](../../../banach-algebra.md#c-star-subalgebra) $C^*(1,h)$ in the [unitization](../../../banach-algebra.md#unitization-of-an-algebra). Its [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) at $h$ equals the ambient [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element): both [Banach algebra spectra](../../../banach-algebra.md#spectrum-of-an-element) are real, the complement of the ambient [compact](../../../topology.md#compact-space) real [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) is [connected](../../../geometry-and-topology.md#connected-space), and the resolvent-component result of Question 1 retains that whole complement in the smaller algebra. [Characters](../../../representation-theory.md#character-of-a-representation) of this [subalgebra](../../../algebra.md#subalgebra) are determined by their values at $h$, so its [character space](../../../banach-algebra.md#character-space-of-an-algebra) is homeomorphic to $\sigma(h)$. We obtain the [continuous functional calculus](../../../banach-algebra.md#continuous-functional-calculus) $C(\sigma(h))\to C^*(1,h)$.

Interpret $\mathbb R^+$ here as $[0,\infty)$. If $\sigma(h)\subseteq[0,\infty)$, apply this calculus to $t\mapsto\sqrt t$, obtaining a Hermitian $k$ with $k^2=h$. In a nonunital algebra this element remains in $A$ because the defining scalar function vanishes at zero. Conversely, if $h=k^2$ with $k=k^*$, [spectral mapping theorem](../../../mathematics.md#spectral-mapping-theorem) and the real [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) of $k$ give $\sigma(h)=\{t^2:t\in\sigma(k)\}\subseteq[0,\infty)$. Hence **nonnegative [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) is equivalent to being the square of a [Hermitian algebra element](../../../associative-algebra.md#hermitian-element-of-a-star-algebra)**. A strict-positive interpretation would exclude $h=0$, and would not be equivalent to the assertion about an arbitrary Hermitian square.

Finally, use the two [continuous](../../../calculus.md#continuous-function) real functions $t\mapsto\sqrt{\max(t,0)}$ and $t\mapsto\sqrt{\max(-t,0)}$ on $\sigma(x)$. Their calculus values $u,v$ are Hermitian, belong to $A$ also in the nonunital case, and satisfy

$$
\boxed{x=u^2-v^2.}
$$

## 4

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Put $K=\sigma(T)$ and use the [continuous functional calculus](../../../banach-algebra.md#continuous-functional-calculus) $\pi:C(K)\to\mathcal B(H)$. It is a [unital](../../../associative-algebra.md#unital-algebra) star-homomorphism taking the coordinate function to $T$. This follows from the commutative C-star theorem applied to $C^*(I,T,T^*)$, together with spectral permanence for [C-star subalgebras](../../../banach-algebra.md#c-star-subalgebra), which is among the permitted C-star results.

Take the [Hilbert space](../../../hilbert-space.md) inner product linear in its first variable. For a [vector](../../../vector-space.md#vector) $\xi$, let $H_\xi=\overline{\{\pi(f)\xi:f\in C(K)\}}$. This cyclic subspace is invariant under every $\pi(f)$ and its adjoint, so it is reducing. The functional $f\mapsto\langle\pi(f)\xi,\xi\rangle$ is positive because $f\ge0$ implies $\pi(f)=\pi(\sqrt f)^*\pi(\sqrt f)$. It has, by the [Riesz-Markov-Kakutani representation theorem](../../../functional-analysis.md#riesz-markov-kakutani-representation-theorem), a finite regular positive [Borel measure](../../../measure-theory.md#borel-measure) $\mu_\xi$ on $K$. The identity

$$
\|\pi(f)\xi\|^2=\int_K|f|^2\,d\mu_\xi
$$

makes $f\mapsto\pi(f)\xi$ an [isometry](../../../riemannian-geometry.md#isometry) on its quotient by the functions of zero $L^2$ [norm](../../../functional-analysis.md#norm). Density of [continuous](../../../calculus.md#continuous-function) functions in $L^2(\mu_\xi)$ extends it to a unitary $U_\xi:L^2(\mu_\xi)\to H_\xi$. Multiplication by a [continuous](../../../calculus.md#continuous-function) function intertwines with $\pi$ on this subspace.

Choose a maximal family of mutually [orthogonal](../../../linear-algebra.md#orthogonal-vectors) nonzero cyclic [reducing subspaces](../../../hilbert-space.md#reducing-subspace-of-a-hilbert-space-operator). Their [orthogonal](../../../linear-algebra.md#orthogonal-vectors) sum is all of $H$: otherwise its reducing [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) contains a nonzero [vector](../../../vector-space.md#vector) generating another such subspace. This argument does not require separability. For a bounded [Borel measurable function](../../../measure-theory.md#borel-measurable-function) $g$ on $K$, multiplication $M_g$ on every $L^2(\mu_\xi)$ is bounded with [norm](../../../functional-analysis.md#norm) at most $\|g\|_\infty$. Define on that [orthogonal](../../../linear-algebra.md#orthogonal-vectors) sum

$$
\boxed{\beta_T(g)=\bigoplus_\xi U_\xi M_gU_\xi^{-1}.}
$$

[Multiplication operators](../../../vector-space.md#multiplication-operator) satisfy $M_{fg}=M_fM_g$, $M_{\overline g}=M_g^*$ and $M_1=I$. The same identities hold for their [direct sums](../../../vector-space.md#direct-sum), and the [norm](../../../functional-analysis.md#norm) bound is uniform in $\xi$. Thus $\beta_T$ is a norm-decreasing [unital](../../../associative-algebra.md#unital-algebra) star-homomorphism on the algebra of actual bounded [Borel measurable functions](../../../measure-theory.md#borel-measurable-function), and $\beta_T(Z)=T$ because it extends $\pi$. No quotient by a single unspecified measure is being substituted for that Borel algebra.

Choose the bounded Borel measurable square root $s(0)=0$ and $s(z)=|z|^{1/2}e^{i\operatorname{Arg}(z)/2}$ for $z\ne0$, taking $\operatorname{Arg}\in[0,2\pi)$. Let $S=\beta_T(s)$. Then

$$
\boxed{S^2=T,\qquad S^*S=\beta_T(|s|^2)=SS^*.}
$$

Thus every bounded [normal operator](../../../hilbert-space.md#normal-operator) has a normal square root. The Borel branch is essential in general: on a circle winding about zero a [continuous](../../../calculus.md#continuous-function) square-root branch need not exist.

## 5

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [representation of a Banach algebra](../../../module-theory.md#representation-of-a-banach-algebra) is a complex-linear multiplicative map $\pi:A\to\operatorname{End}_{\mathbb C}(X)$. A nonzero irreducible action of a [unital algebra](../../../associative-algebra.md#unital-algebra) automatically has $\pi(1)=I$: the image of the idempotent $\pi(1)$ is a nonzero invariant subspace and hence is all of $X$. An [algebraically irreducible representation of a Banach algebra](../../../module-theory.md#algebraically-irreducible-representation-of-a-banach-algebra) is a nonzero action if it has no nonzero proper [invariant submodule](../../../module-theory.md#invariant-submodule), whether [closed](../../../topology.md#closed-set) or not. A [normed representation of a Banach algebra](../../../module-theory.md#normed-representation-of-a-banach-algebra) has $\pi(a)$ bounded for each $a$ on a preassigned [normed vector space](../../../functional-analysis.md#normed-vector-space) $X$; [continuity](../../../calculus.md#continuous-function) of $\pi$ as an operator-norm-valued map is a further conclusion. This must not be confused with topological irreducibility, which excludes only [closed](../../../topology.md#closed-set) [invariant subspaces](../../../representation-theory.md#invariant-subspace). Unitizing the algebra extends a nonunital action by $\pi(a+\lambda1)=\pi(a)+\lambda I$, so it is enough to discuss the [unital](../../../associative-algebra.md#unital-algebra) case.

For $\xi\ne0$, irreducibility gives $A\xi=X$. The annihilator $L_\xi=\{a:\pi(a)\xi=0\}$ is a [maximal left ideal](../../../associative-algebra.md#maximal-left-ideal): an intermediate [left ideal](../../../associative-algebra.md#left-ideal) gives an intermediate [submodule](../../../module-theory.md#submodule) of $X$. It is [closed](../../../topology.md#closed-set) by the Neumann-series argument for [maximal left ideals](../../../associative-algebra.md#maximal-left-ideal). Consequently $A/L_\xi$ transports a complete quotient [norm](../../../functional-analysis.md#norm) to $X$, and left multiplication is contractive in this [norm](../../../functional-analysis.md#norm). Every [algebraically irreducible representation of a Banach algebra](../../../module-theory.md#algebraically-irreducible-representation-of-a-banach-algebra) can therefore be realized continuously on a [Banach space](../../../banach-space.md). This alone does not prove [continuity](../../../calculus.md#continuous-function) for its preassigned [norm](../../../functional-analysis.md#norm).

The kernel of $\pi$ is the intersection of the [closed](../../../topology.md#closed-set) [left ideals](../../../associative-algebra.md#left-ideal) $L_\xi$ and is a [closed](../../../topology.md#closed-set) [primitive ideal](../../../associative-algebra.md#primitive-ideal). The [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) is the intersection of all [primitive ideals](../../../associative-algebra.md#primitive-ideal), equivalently the intersection of [maximal left ideals](../../../associative-algebra.md#maximal-left-ideal). Thus these quotient representations detect semisimplicity. Equivalent [algebra representations](../../../module-theory.md#representation-of-an-associative-algebra) are related by a bijective [module homomorphism](../../../module-theory.md#module-homomorphism).

The algebra of [module endomorphisms](../../../module-theory.md#module-endomorphism) is exactly $\mathbb C I$. Indeed, if a [module endomorphism](../../../module-theory.md#module-endomorphism) $D$ sends a fixed cyclic [vector](../../../vector-space.md#vector) $\xi$ to $a\xi$, then $D(b\xi)=ba\xi$. It is induced by bounded right multiplication by $a$ on $A/L_\xi$, so is bounded for the [quotient norm on an irreducible Banach module](../../../module-theory.md#quotient-norm-on-an-irreducible-banach-module). Every nonzero [module endomorphism](../../../module-theory.md#module-endomorphism) is injective and surjective by irreducibility, and its inverse is bounded by the same argument. This [commutant of an operator algebra](../../../associative-algebra.md#commutant-of-an-operator-algebra) is a [closed](../../../topology.md#closed-set) division [subalgebra](../../../algebra.md#subalgebra) of the [bounded operators](../../../topological-vector-space.md#continuous-linear-operator) on this Banach module; the [Gelfand-Mazur theorem](../../../banach-algebra.md#gelfand-mazur-theorem) makes it $\mathbb C I$.

The [Jacobson density theorem](../../../noncommutative-algebra.md#jacobson-density-theorem) now says that for finitely many [linearly independent](../../../vector-space.md#linear-independence) $\xi_1,\ldots,\xi_n$ and arbitrary $\eta_1,\ldots,\eta_n$, one element of $A$ sends all $\xi_j$ to $\eta_j$. Here is the induction behind it. The one-vector assertion is $A\xi_1=X$. Assuming the first $n-1$ coordinates can be prescribed, set $L=\{a:a\xi_j=0\ (j<n)\}$. Its image $L\xi_n$ is an [invariant subspace](../../../representation-theory.md#invariant-subspace). If it is $X$, it adjusts the last image without changing the first ones. If it is zero, the rule $(a\xi_1,\ldots,a\xi_{n-1})\mapsto a\xi_n$ is a well-defined module map $X^{n-1}\to X$. Each coordinate map is scalar by the [module endomorphism](../../../module-theory.md#module-endomorphism) result, forcing $\xi_n$ to be a [linear combination](../../../vector-space.md#linear-combination) of the earlier [vectors](../../../vector-space.md#vector), a contradiction. This proves the assertion.

We can now give Johnson's [continuity](../../../calculus.md#continuous-function) argument with its crucial construction. If $X$ is finite dimensional, the [closed](../../../topology.md#closed-set) kernel has finite codimension and $A/\ker\pi$ is finite dimensional, so $\pi$ is [continuous](../../../calculus.md#continuous-function). Suppose instead that $X$ is infinite dimensional. Let

$$
Y=\{\xi\in X:a\mapsto\pi(a)\xi\text{ is continuous}\}.
$$

This is an [invariant submodule](../../../module-theory.md#invariant-submodule), because the orbit map of $\pi(b)\xi$ is the orbit map of $\xi$ composed with the bounded map $a\mapsto ab$. Thus either $Y=X$ or $Y=0$.

To rule out $Y=0$, choose [linearly independent](../../../vector-space.md#linear-independence) unit [vectors](../../../vector-space.md#vector) $\xi_0,\xi_1,\ldots$. There are elements $a_n\in A$ such that, with $c_n=a_n\cdots a_1$,

$$
\pi(c_m)\xi_n=0\quad(m>n),\qquad
\{\pi(c_n)\xi_j:j\ge n\}\text{ is linearly independent}.
$$

For completeness, construct them in the canonical quotient-norm Banach module. At stage $n$ the current tail [vectors](../../../vector-space.md#vector) are independent. In the [closed](../../../topology.md#closed-set) left annihilator of its first [vector](../../../vector-space.md#vector), density permits arbitrary images of any finite list of the remaining [vectors](../../../vector-space.md#vector). The condition that finitely many such images are independent is [open](../../../topology.md#open-set) in this Banach subspace and dense: perturb any element by $t$ times an element prescribing independent images; a suitable determinant is a nonzero [polynomial](../../../polynomial.md) in $t$, with only finitely many exceptional values. The [Baire category theorem](../../../topological-analysis.md#baire-category-theorem) intersects these [open](../../../topology.md#open-set) dense conditions for all initial finite tail lists. The resulting $a_n$ kills the first current [vector](../../../vector-space.md#vector) and retains independence of the entire remaining tail. This is the [countable annihilation sequence in an irreducible Banach module](../../../module-theory.md#countable-annihilation-sequence-in-an-irreducible-banach-module).

The [gliding-hump continuity principle](../../../functional-analysis.md#gliding-hump-continuity-principle) supplies the other ingredient: if $E,F$ are [Banach spaces](../../../banach-space.md), $S:E\to F$ is linear, $T_j:E\to E$ and $U_n:F\to F_n$ are bounded, and $U_nST_1\cdots T_m$ is [continuous](../../../calculus.md#continuous-function) whenever $m>n$, then $U_nST_1\cdots T_n$ is [continuous](../../../calculus.md#continuous-function) eventually. The product form of this principle is recorded in [Proposition 1.3 of Thomas's paper](https://msp.org/pjm/1993/159-1/pjm-v159-n1-p08-p.pdf). Here is the contradiction mechanism. Rescale so $\|T_j\|,\|U_n\|\le1$ and put $P_m=T_1\cdots T_m$. If infinitely many diagonal maps are discontinuous, choose increasing $n_j$ and successively tiny $x_j$ so

$$
\|U_{n_j}SP_{n_j}x_j\|>j+1+\sum_{i<j}\|U_{n_j}SP_{n_i}x_i\|.
$$

Also choose $\|x_j\|\le2^{-j}/(1+\max_{i<j}\|U_{n_i}SP_{n_i+1}\|)$. The convergent sum $x=\sum_jP_{n_j}x_j$ has, after its $j$th term, a tail factoring through $P_{n_j+1}$. Applying that [continuous](../../../calculus.md#continuous-function) composite bounds the tail contribution by one. The display forces $\|U_{n_j}Sx\|>j$, contradicting $\|U_{n_j}Sx\|\le\|Sx\|$. Only finite decompositions and the [continuous](../../../calculus.md#continuous-function) tail composites are used; no unjustified interchange of a discontinuous map with an infinite sum occurs.

Apply this principle with $E=A$, $F=\mathcal B(\overline X)$, where $\overline X$ is the completion in the original [norm](../../../functional-analysis.md#norm), and $S(a)$ the bounded extension of $\pi(a)$. Set $T_j(a)=aa_j$ and $U_n(R)=R\xi_n$. Then

$$
U_nST_1\cdots T_m(a)=\pi(a)\pi(a_m\cdots a_1)\xi_n.
$$

For $m>n$ this is zero, hence [continuous](../../../calculus.md#continuous-function). For $m=n$ it is the orbit map of a nonzero [vector](../../../vector-space.md#vector), hence discontinuous if $Y=0$. This contradicts the principle. Therefore $Y=X$.

Finally, apply the [Uniform boundedness principle](../../../banach-space.md#uniform-boundedness-principle) on the [Banach space](../../../banach-space.md) $A$ to the [continuous](../../../calculus.md#continuous-function) maps $a\mapsto\pi(a)\xi$ indexed by $\|\xi\|\le1$. They are pointwise bounded because each individual $\pi(a)$ is bounded in the original [norm](../../../functional-analysis.md#norm). It gives

$$
\boxed{\|\pi(a)\|\le C\|a\|\quad(a\in A).}
$$

This proves [Johnson's continuity theorem for irreducible normed representations](../../../module-theory.md#johnson-s-continuity-theorem-for-irreducible-normed-representations), including when the original [normed vector space](../../../functional-analysis.md#normed-vector-space) is incomplete. The quotient [norm](../../../functional-analysis.md#norm), countable density construction, and gliding hump explain the substantive steps rather than assuming the desired [continuity](../../../calculus.md#continuous-function) in advance.

## 6

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

We first extend the scalar [Hadamard three-circle theorem](../../../complex-analysis.md#hadamard-three-circle-theorem) to a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) Banach-space-valued function $F$. Apply its inequality to $\ell(F(z))$ for every [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) $\ell$ of [norm](../../../functional-analysis.md#norm) at most one, and use the [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) to recover the [norm](../../../functional-analysis.md#norm). For the radii $1/R,1,R$ this gives

$$
\|F(1)\|^2\le\sup_{|z|=R}\|F(z)\|\;\sup_{|z|=1/R}\|F(z)\|.
$$

Now take $F(z)=p(z)^{2^n}$. Even for noncommuting coefficients this is an algebra-valued [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) [polynomial](../../../polynomial.md). Taking the $2^{-n}$th power gives

$$
\|p(1)^{2^n}\|^{2/2^n}\le
\max_{|z|=R}\|p(z)^{2^n}\|^{1/2^n}
\max_{|z|=1/R}\|p(z)^{2^n}\|^{1/2^n}.
$$

On each [boundary](../../../topology.md#boundary-of-a-set) circle the [continuous](../../../calculus.md#continuous-function) functions $f_n(z)=\|p(z)^{2^n}\|^{1/2^n}$ decrease, by submultiplicativity, to $r_A(p(z))$ by the [spectral radius formula](../../../analysis.md#spectral-radius-formula). Their maxima decrease to the [supremum](../../../real-analysis.md#supremum) of this [pointwise limit](../../../real-analysis.md#pointwise-limit). To justify that passage without assuming [continuity](../../../calculus.md#continuous-function) of the [spectral radius](../../../analysis.md#spectral-radius), take maximizing points along a convergent subsequence on the [compact](../../../topology.md#compact-space) circle. For any fixed $k$, all later $f_n$ are bounded by $f_k$; [continuity](../../../calculus.md#continuous-function) of $f_k$ therefore bounds the limiting maxima by $f_k$ at the limiting point. Taking the infimum over $k$ gives the desired upper bound, while the reverse bound is immediate.

Passing to the limit proves the [spectral-radius three-circle inequality](../../../analysis.md#spectral-radius-three-circle-inequality) at the geometric mean:

$$
\boxed{r_A(p(1))^2\le
\sup_{|z|=R}r_A(p(z))\;\sup_{|z|=1/R}r_A(p(z)).}
$$

For a nonunital algebra, use its [unitization of an algebra](../../../banach-algebra.md#unitization-of-an-algebra); the [spectral radius](../../../analysis.md#spectral-radius) of an original algebra element is unchanged. Zero [boundary](../../../topology.md#boundary-of-a-set) suprema cause no difficulty in the decreasing-limit argument.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

It suffices first to treat [unital algebras](../../../associative-algebra.md#unital-algebra) and a [unital](../../../associative-algebra.md#unital-algebra) [homomorphism](../../../algebra.md#homomorphism). A surjective [homomorphism](../../../algebra.md#homomorphism) between [unital algebras](../../../associative-algebra.md#unital-algebra) automatically preserves the identity. If $B=0$, [continuity](../../../calculus.md#continuous-function) is immediate. In the nonunital case, extend to the forced [unitizations](../../../banach-algebra.md#unitization-of-an-algebra) by $T^+(a+\lambda1)=T(a)+\lambda1$. This is still surjective and the [unitization](../../../banach-algebra.md#unitization-of-an-algebra) of a semisimple algebra is semisimple: its radical projects to zero in its scalar quotient, and its remaining intersection with the original algebra is its original radical. [Continuity](../../../calculus.md#continuous-function) of the extension implies [continuity](../../../calculus.md#continuous-function) of the original map.

An [algebra homomorphism](../../../algebra.md#algebra-homomorphism-over-a-field) decreases the [spectral radius](../../../analysis.md#spectral-radius), even without any [continuity](../../../calculus.md#continuous-function) assumption, because it takes an inverse of $\lambda1-a$ to an inverse of $\lambda1-T(a)$. Suppose $a_n\to0$ in $A$ and $T(a_n)\to b$ in $B$. Fix any $c\in B$ and choose $u,v\in A$ with $T(u)=b$, $T(v)=c$. Put

$$
w=vu,\quad w_n=va_n,\quad d=T(w)=cb,\quad d_n=T(w_n)\longrightarrow d.
$$

Consider the [polynomial](../../../polynomial.md) $q_n(z)=T((1-z)w_n+zw)=(1-z)d_n+zd$. Its value at one is exactly $d$. On the outer circle $|z|=R$,

$$
r_B(q_n(z))\le\|q_n(z)\|\le\|d\|+(1+R)\|d_n-d\|.
$$

On the inner circle $|z|=1/R$, spectral-radius decrease gives

$$
r_B(q_n(z))\le r_A((1-z)w_n+zw)
\le(1+1/R)\|w_n\|+\|w\|/R.
$$

Applying part (i) in $B$ and then letting $n\to\infty$, with $R$ fixed, gives

$$
r_B(cb)^2\le\frac{\|cb\|\|vu\|}{R}.
$$

This holds for every $R>1$, so **$r_B(cb)=0$ for every $c\in B$**.

This forces $b$ into the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical). To see the criterion directly, if $b$ were outside a [maximal left ideal](../../../associative-algebra.md#maximal-left-ideal) $L$, then $L+Bb=B$, so $1=l+cb$ for some $l\in L$, $c\in B$. The equality $r_B(cb)=0$ makes $1-cb$ invertible, but this element equals $l\in L$, impossible in a proper [left ideal](../../../associative-algebra.md#left-ideal). Hence $b$ lies in every [maximal left ideal](../../../associative-algebra.md#maximal-left-ideal). Since $B$ is semisimple, $b=0$.

We have shown that the separating space of $T$ is zero. If $a_n\to a$ and $T(a_n)\to y$, apply the result to $a_n-a$ to obtain $y=T(a)$. Its graph is [closed](../../../topology.md#closed-set), and the [closed graph theorem](../../../functional-analysis.md#closed-graph-theorem) now proves

$$
\boxed{T\text{ is continuous}.}
$$

The crucial estimate uses part (i) with an exactly fixed central value; it does not assume the false general assertion that the [spectral radius](../../../analysis.md#spectral-radius) is [continuous](../../../calculus.md#continuous-function) under [norm](../../../functional-analysis.md#norm) limits.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
