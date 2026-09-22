<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A smooth right [group action](../../../../../group-action.md) is a [smooth map](../../../../../smooth-map-between-manifolds.md) $(p,g)\mapsto p\cdot g$ from $P\times G$ to $P$, with $p\cdot e=p$ and $(p\cdot g)\cdot h=p\cdot(gh)$. It is a [free action of a group](../../../../../free-action-of-a-group.md) if $p\cdot g=p$ implies $g=e$.

A smooth [principal bundle](../../../../../principal-bundle.md) consists of such a free action and a surjective map $\pi:P\to B$ whose fibres are the orbits, together with equivariant [local trivializations](../../../../../local-trivialization.md)

$$
\Phi:\pi^{-1}(N)\longrightarrow N\times G,
\qquad \operatorname{pr}_1\Phi=\pi,
\qquad \Phi(p\cdot h)=\Phi(p)\cdot h,
$$

where $(x,g)\cdot h=(x,gh)$. The trivializations are [diffeomorphisms](../../../../../diffeomorphism.md); in particular the bundle projection is a [submersion](../../../../../submersion.md).

For two such trivializations, $H=\Phi_2\Phi_1^{-1}$ fixes the base coordinate and is equivariant. Write $H(x,e)=(x,\psi(x))$. Equivariance immediately gives

$$
\boxed{H(x,g)=H((x,e)\cdot g)=(x,\psi(x)g).}
$$

The function $\psi$ is smooth because $x\mapsto(x,e)$ and $H$ are smooth. This proves the general [transition function of a principal bundle](../../../../../transition-function-of-a-principal-bundle.md) formula; the multiplier is on the left, even though the original action is on the right.

For the explicit bundle, represent a point of $\mathbb{RP}^3$ by a nonzero vector $w=(w_1,w_2)\in\mathbb C^2$ modulo nonzero real scaling. The map sends $[w]$ to the complex line $[w_1:w_2]$, so it is well-defined and surjective. Its smoothness follows from the local ratio charts below. Ordinary scalar multiplication by $u\in U(1)$ would not be free, since $u=-1$ acts trivially on real projective classes. Instead define

$$
\boxed{[w]\cdot u=[\lambda w],\qquad \lambda\in U(1),\quad\lambda^2=u.}
$$

The two possible roots differ by a real sign, so give the same class. This is independent of the real representative of $[w]$. Products of chosen roots show the right action law, and the identity acts trivially. Locally on $U(1)$ a smooth square-root branch exists; these local definitions agree projectively and prove global smoothness of the action.

If $[\lambda w]=[w]$, then $\lambda w=rw$ for some nonzero real $r$. Since $w\ne0$ and $|\lambda|=1$, this forces $\lambda=\pm1$ and hence $u=1$. The action is free. Two points in the same fibre have representatives $w'=cw$ for some $c\in\mathbb C^*$; absorb $|c|$ into the real scaling and use $u=(c/|c|)^2$. Thus the orbits are exactly the fibres.

Let $N_1=\{[z:1]\}$ and $N_2=\{[1:\zeta]\}$. Using these base coordinates, define

$$
\begin{aligned}
\Phi_1([w_1,w_2])&=\left(\frac{w_1}{w_2},\left(\frac{w_2}{|w_2|}\right)^2\right)\quad(w_2\ne0),\\
\Phi_2([w_1,w_2])&=\left(\frac{w_2}{w_1},\left(\frac{w_1}{|w_1|}\right)^2\right)\quad(w_1\ne0).
\end{aligned}
$$

Both formulas are invariant under real nonzero scaling, including negative scaling. Their inverses are

$$
\Phi_1^{-1}(z,u)=[\lambda z,\lambda],\qquad
\Phi_2^{-1}(\zeta,u)=[\lambda,\lambda\zeta],\qquad\lambda^2=u.
$$

Again the sign of the root does not matter. Direct substitution shows they are two-sided inverses. The forward maps are smooth, and local square-root branches prove that the inverses are smooth. Under the right action, each squared phase is multiplied by $u$, so the maps are equivariant. They are therefore genuine principal trivializations of the [principal circle bundle on real projective three-space](../../../../../principal-circle-bundle-on-real-projective-three-space.md).

On the overlap $z\ne0$, we have $\zeta=1/z$ and

$$
\left(\frac{w_1}{|w_1|}\right)^2
=\left(\frac{z}{|z|}\right)^2\left(\frac{w_2}{|w_2|}\right)^2.
$$

Consequently

$$
\boxed{\Phi_2\Phi_1^{-1}(z,u)=\left(\frac1z,\frac{z}{\overline z}u\right),
\qquad\psi_{21}(z)=\frac{z}{\overline z}.}
$$

When the base point itself, rather than its chart coordinate, is written as $x$, its coordinate remains $x$ in the general transition formula. The opposite transition has reciprocal multiplier. The doubled phase is essential to freeness and is not the ordinary Hopf-bundle phase.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
