<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a densely defined closed operator $S$, define its [lower norm](../../../../../lower-norm-of-an-operator.md)

$$
\nu(S)=\inf_{\substack{x\in D(S)\\\|x\|=1}}\|Sx\|,
\qquad
\mu(S)=\min\{\nu(S),\nu(S^*)\}.
$$

The closed-range theorem gives

$$
\boxed{
\mu(S)=
\begin{cases}
\|S^{-1}\|^{-1},&S\text{ is bijective},\\
0,&S\text{ is not bijective}.
\end{cases}}
$$

Therefore

$$
\operatorname{Sp}(T)=\{z:\mu(T(z))=0\},
$$

and

$$
\operatorname{Sp}_\epsilon(T)
=\operatorname{Cl}\{z:\mu(T(z))<\epsilon\}.
$$

We next show that $\mu(T(z))$ is accessible through the matrix-entry evaluations. Put $L_n=\operatorname{span}\{e_1,\ldots,e_n\}$ and define

$$
\nu_n(T(z))
=\inf_{\substack{x\in L_n\\\|x\|=1}}\|T(z)x\|,
\qquad
\nu_n(T(z)^*)
=\inf_{\substack{x\in L_n\\\|x\|=1}}\|T(z)^*x\|.
$$

Because the canonical span is a core for both operators,

$$
\nu_n(T(z))\downarrow\nu(T(z)),
\qquad
\nu_n(T(z)^*)\downarrow\nu(T(z)^*).
$$

For fixed $m,n$ and grid point $z$, form

$$
M_{m,n}(z)
=\left(\langle T(z)e_j,e_i\rangle\right)_
{\substack{1\leq i\leq m\\1\leq j\leq n}}.
$$

Its entries belong to $\Lambda$. The smallest singular value of $M_{m,n}(z)$ increases as $m\to\infty$ to $\nu_n(T(z))$. Applying the same construction to the conjugate-transposed entries gives $\nu_n(T(z)^*)$. Thus two nested finite-matrix limits determine $\mu(T(z))$.

The assumed gap continuity of $T$ and the identity

$$
\widehat\delta(T(z)^*,T(w)^*)
=\widehat\delta(T(z),T(w))
$$

make the corresponding lower-norm tests stable under movement of $z$. The rational grids $G_n$ become dense on every bounded disk. Hence an arithmetic algorithm can, on $G_n\cap\overline B_n(0)$, use the two finite-section levels above and a vanishing rational tolerance to output all grid cells certified by

$$
\mu(T(z))<\epsilon.
$$

Taking their closures and letting the mesh and tolerance vanish converges in the [Attouch--Wets topology](../../../../../attouch-wets-topology.md) to

$$
\operatorname{Cl}\{z:\mu(T(z))<\epsilon\}
=\operatorname{Sp}_\epsilon(T).
$$

The strict existential inequality requires two nested limits, with approximants entering from the prescribed side. In the notation of the arithmetic hierarchy this proves

$$
\boxed{
\{\operatorname{Sp}_\epsilon,\Omega_{\rm NL},
\operatorname{MAW},\Lambda\}\in\Sigma_2^A}.
$$

For the spectrum, equality to zero is the countable intersection

$$
\{z:\mu(T(z))=0\}
=\bigcap_{q=1}^\infty
\{z:\mu(T(z))<1/q\}.
$$

Use the preceding two-level pseudospectral procedure with threshold $1/q$, and add an outer limit $q\to\infty$. Outer approximants remove every point with positive lower norm, while gap continuity and density of the grids retain every zero. Truncating to expanding disks and using vanishing mesh again gives Attouch–Wets convergence. The universal outer intersection reverses the one-sided classification and adds one level, proving

$$
\boxed{
\{\operatorname{Sp},\Omega_{\rm NL},
\operatorname{MAW},\Lambda\}\in\Pi_3^A}.
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 358](../../paper-358-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
