<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Riemann mapping theorem](../../../../../riemann-mapping-theorem.md) asserts that a nonempty [simply connected domain](../../../../../simply-connected-domain.md) $\Omega\subsetneq\mathbb C$ is [biholomorphic](../../../../../biholomorphism.md) to the [unit disk](../../../../../unit-disk.md) $\mathbb D$. More precisely, for each $z_0\in\Omega$ there is a unique [biholomorphism](../../../../../biholomorphism.md) $f:\Omega\to\mathbb D$ satisfying $f(z_0)=0$ and $f'(z_0)>0$. We prove existence through an extremal derivative, deriving the compactness and injectivity steps rather than assuming special lemmas for the theorem.

First construct a bounded [univalent function](../../../../../univalent-function.md) on $\Omega$. Choose $a\notin\Omega$ and a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) of $z-a$, which exists by the permitted logarithm result on the translated [simply connected domain](../../../../../simply-connected-domain.md). Put

$$
u(z)=\exp\left(\frac12\log(z-a)\right).
$$

Then $u(z)^2=z-a$, so $u$ is univalent and never zero. Its image $G=u(\Omega)$ is open, and $G\cap(-G)=\varnothing$: equality $u(x)=-u(y)$ would imply $x=y$ after squaring and then $u(x)=0$.

Fix $w_0\in G$ and choose $r>0$ with $B(w_0,r)\subset G$. It follows that $B(-w_0,r)\subset-G$ is disjoint from $G$, so $|u(z)+w_0|\ge r$ throughout $\Omega$. Hence

$$
h(z)=\frac{r}{2(u(z)+w_0)}
$$

is a [univalent function](../../../../../univalent-function.md) with $|h|\le1/2$. For $b\in\mathbb D$, define

$$
T_b(w)=\frac{w-b}{1-\overline b w}.
$$

The identity

$$
1-|T_b(w)|^2=\frac{(1-|b|^2)(1-|w|^2)}{|1-\overline b w|^2}
$$

and the inverse $T_b^{-1}(w)=(w+b)/(1+\overline b w)$ show directly that $T_b$ is an [automorphism of the unit disk](../../../../../automorphism-of-the-unit-disk.md). Apply $T_{h(z_0)}$ to $h$ and then a rotation to make its nonzero derivative at $z_0$ positive. The family $\mathcal A$ of univalent maps $\Omega\to\mathbb D$ with value zero and positive derivative at $z_0$ is therefore nonempty.

Let

$$
M=\sup\{v'(z_0):v\in\mathcal A\}.
$$

It is positive. Choose $\rho>0$ with $\overline{B(z_0,\rho)}\subset\Omega$. The [Cauchy estimate](../../../../../cauchy-estimate.md) gives $v'(z_0)\le1/\rho$ for every $v\in\mathcal A$, so $M$ is finite. Take a sequence $v_j\in\mathcal A$ with $v_j'(z_0)\to M$.

We now justify a [locally uniform convergence](../../../../../locally-uniform-convergence.md) subsequence. On any compact subset of $\Omega$, the bound $|v_j|\le1$ and the [Cauchy estimate](../../../../../cauchy-estimate.md) on slightly larger interior disks give a uniform derivative bound. They therefore give [equicontinuity](../../../../../equicontinuity.md). Apply the [Arzelà-Ascoli theorem](../../../../../arzela-ascoli-theorem.md) on a compact exhaustion of $\Omega$, then take a [diagonal subsequence for locally uniform convergence](../../../../../diagonal-subsequence-for-locally-uniform-convergence.md). Its limit $v$ is holomorphic: pass to the limit in the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) on every small interior circle. The same formula for derivatives gives

$$
v(z_0)=0,\qquad v'(z_0)=M>0.
$$

Thus $v$ is nonconstant. Initially $|v|\le1$, and the [maximum modulus principle](../../../../../maximum-modulus-principle.md) improves this to $|v|<1$ everywhere.

For completeness, the needed [locally uniform limit of univalent functions](../../../../../locally-uniform-limit-of-univalent-functions.md) argument is short. If $x\ne y$ and $v(x)=v(y)$, the nonconstant holomorphic function $v-v(y)$ has an isolated zero at $x$. Choose a small closed disk around $x$ excluding $y$, with no zero on its boundary. Uniform convergence there gives $v_j-v_j(y)\to v-v(y)$. The [Rouche theorem](../../../../../rouche-s-theorem.md) then makes $v_j-v_j(y)$ have a zero inside that disk for all sufficiently large $j$. Its only possible zero, by injectivity of $v_j$, is $y$, outside the disk. This contradiction proves injectivity of $v$. Therefore $v\in\mathcal A$ and attains the supremum $M$.

It remains to prove surjectivity. Suppose $c\in\mathbb D$ is omitted by $v$; since $v(z_0)=0$, necessarily $c\ne0$. The domain $T_c(v(\Omega))$ is simply connected, because both constituent maps are homeomorphisms onto their images, and it excludes zero. The permitted [holomorphic logarithm](../../../../../holomorphic-logarithm.md) gives a [holomorphic square root](../../../../../holomorphic-square-root.md)

$$
g(z)=\exp\left(\frac12\operatorname{Log}(T_c(v(z)))\right).
$$

This maps $\Omega$ into $\mathbb D$ and is univalent, since equality of its values implies equality after squaring and hence equality of the original arguments. Write $\gamma=g(z_0)$. Then $\gamma^2=T_c(0)=-c$ and $|\gamma|=\sqrt{|c|}$. Normalize again with $V=T_\gamma\circ g$ and a rotation. Its derivative magnitude is

$$
\begin{aligned}
|V'(z_0)|
&=\frac1{1-|\gamma|^2}\frac{|T_c'(0)|}{2|\gamma|}\,v'(z_0)\\
&=\frac{1-|c|^2}{2\sqrt{|c|}(1-|c|)}M
=\frac{1+|c|}{2\sqrt{|c|}}M>M.
\end{aligned}
$$

The strict inequality follows from $(1-\sqrt{|c|})^2>0$. This [square-root improvement of a normalized conformal map](../../../../../square-root-improvement-of-a-normalized-conformal-map.md) contradicts extremality. Thus $v(\Omega)=\mathbb D$. An injective holomorphic map has nonzero derivative and a holomorphic local inverse; these inverses agree, so the resulting bijection is biholomorphic. We have proved existence.

For uniqueness, two normalized maps give an [automorphism of the unit disk](../../../../../automorphism-of-the-unit-disk.md) $v_2\circ v_1^{-1}$ fixing zero. Apply the [Schwarz lemma](../../../../../schwarz-lemma.md), proved in the next part, to this automorphism and its inverse. Both inequalities force equality, so the equality case makes it a rotation. Its derivative at zero is the positive real number $v_2'(z_0)/v_1'(z_0)$, forcing that rotation to be the identity. Therefore

$$
\boxed{\text{there is exactly one normalized biholomorphism }\Omega\to\mathbb D}.
$$

The proper-domain hypothesis is necessary: a bounded entire holomorphic function has derivative at most $1/R$ on disks of arbitrarily large radius by the [Cauchy estimate](../../../../../cauchy-estimate.md), and hence is constant. Conversely, a domain biholomorphic to the disk is simply connected because the map is a homeomorphism.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
