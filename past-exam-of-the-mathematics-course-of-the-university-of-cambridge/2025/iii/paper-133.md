# Paper 133

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_133.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_133.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 133](paper-133.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a finite [group presentation](../../../geometric-group-theory.md#group-presentation) $\langle S\mid R\rangle$ and a word $w\in F(S)$ representing the identity, the [area of a null-homotopic word](../../../geometric-group-theory.md#area-of-a-null-homotopic-word) is

$$
\operatorname{Area}(w)=
\min\left\{N:w=\prod_{i=1}^N u_i r_i^{\varepsilon_i}u_i^{-1},\ r_i\in R,\ \varepsilon_i\in\{-1,1\}\right\}.
$$

The [Dehn function](../../../geometric-group-theory.md#dehn-function) of the presentation is

$$
\delta(n)=\max\{\operatorname{Area}(w):w=1\text{ in }G,\ |w|_S\leq n\}.
$$

Equivalently, area is the least number of two-cells in a van Kampen diagram for $w$, and the Dehn function is the worst such area among null words of length at most $n$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [normal form theorem for an amalgamated free product](../../../geometric-group-theory.md#normal-form-theorem-for-an-amalgamated-free-product) says that, after choosing left coset representatives for $C$ in $A$ and $B$, each element of $A*_CB$ has a unique normal form consisting of an initial element of $C$ followed by an alternating word in nontrivial representatives from the two factors. In particular, every nonempty reduced alternating word whose syllables lie outside $C$ is nonidentity.

For the [free product](../../../algebraic-topology.md#free-product) $A*B$, the amalgamated subgroup is trivial. Hence

$$
g=a_1b_1a_2\cdots a_kb_k
$$

is nontrivial whenever, after omitting a possibly empty initial or final syllable, every displayed $A$-syllable and $B$-syllable is nonidentity. It is then a nonempty reduced normal form.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [infinite dihedral group](../../../representation-theory.md#infinite-dihedral-group) is $D_\infty\cong C_2*C_2$, with factors $A=\langle a\rangle$ and $B=\langle b\rangle$. Its [Bass-Serre tree](../../../geometric-group-theory.md#bass-serre-tree) has vertex set

$$
D_\infty/A\sqcup D_\infty/B
$$

and one edge indexed by each $g\in D_\infty$, joining $gA$ to $gB$. Since both factors have order two, every vertex has degree two. The connected tree is therefore a bi-infinite line.

The action is cocompact, and its vertex stabilizers are the finite conjugates of $A$ and $B$, so it is proper. By the [Milnor–Švarc lemma](../../../geometric-group-theory.md#milnor-svarc-lemma), an orbit map from $D_\infty$ with a [word metric](../../../geometric-group-theory.md#word-metric) to this line is a [quasi-isometry](../../../geometric-group-theory.md#quasi-isometry). A simplicial bi-infinite line is quasi-isometric to $\mathbb R$, hence so is $D_\infty$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Map both $a$ and $b$ to the nonidentity element of $C_2$. Both relators $a^2,b^2$ map to the identity, so this gives a homomorphism $D_\infty\to C_2$. A word of length $n$ maps to the parity class of $n$; consequently a null word has even length.

Now let $w$ be a null word of positive even length. Interpreting $a^{-1}=a$ and $b^{-1}=b$, the [free-product normal form theorem](../../../geometric-group-theory.md#normal-form-theorem-for-an-amalgamated-free-product) says that a nonempty alternating word cannot be trivial. Thus $w$ has two adjacent equal letters. Delete this $a^2$ or $b^2$, using one conjugate of a defining relator, and apply induction to the resulting null word of length $n-2$. This gives

$$
\boxed{\operatorname{Area}(w)\leq1+\frac{n-2}{2}=\frac n2.}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Part d gives $\delta(2n)\leq n$. For the reverse inequality, consider $w=a^{2n}$. Under the homomorphism $F(a,b)\to\mathbb Z$ with $a\mapsto1$ and $b\mapsto0$, every conjugate of $a^{\pm2}$ has image $\pm2$ and every conjugate of $b^{\pm2}$ has image zero. Any expression of $a^{2n}$ as a product of conjugates of relators therefore uses at least $n$ factors. Hence

$$
\operatorname{Area}(a^{2n})\geq n.
$$

The opposite inequality follows by applying $a^2$ exactly $n$ times, so the [Dehn function](../../../geometric-group-theory.md#dehn-function) satisfies $\delta(2n)=n$.

## 2

↑ **Parent:** [Paper 133](paper-133.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $x,y\in\operatorname{Fix}(\phi)$. A [tree](../../../combinatorics.md#tree-graph-theory) has a unique geodesic segment $[x,y]$. The isometry $\phi$ sends this segment to the segment $[\phi x,\phi y]=[x,y]$. An isometry of a segment that fixes both endpoints fixes every point of it, so

$$
[x,y]\subseteq\operatorname{Fix}(\phi).
$$

**Thus the fixed-point set of an [elliptic isometry of a tree](../../../geometric-group-theory.md#elliptic-isometry-of-a-tree) is a convex subtree, in particular it is [path-connected](../../../geometry-and-topology.md#path-connected-space).**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $A=\operatorname{Axis}(\phi)$ and let $p$ be the nearest-point projection of $x$ to $A$. If the translation length is $\tau>0$, the unique path from $x$ to $\phi x$ is the concatenation

$$
[x,p]\cup[p,\phi p]\cup[\phi p,\phi x].
$$

The first and last pieces both have length $d(x,A)$, while the middle one has length $\tau$. Therefore

$$
d(x,\phi x)=\tau+2d(x,A).
$$

The displacement is minimized exactly when $x\in A$, proving that the axis is the minimum set of the [displacement function](../../../geometric-group-theory.md#displacement-function).

On $A$, the power $\phi^r$ translates through $r\tau$ when $r>0$ and in the opposite direction through $|r|\tau$ when $r<0$. The same formula applied to $\phi^r$ shows that its minimum set is $A$. Hence

$$
\boxed{\operatorname{Axis}(\phi^r)=\operatorname{Axis}(\phi)
\qquad(r\ne0).}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Suppose that $a$ acted as a [hyperbolic isometry of a tree](../../../geometric-group-theory.md#hyperbolic-isometry-of-a-tree), with [translation length](../../../geometric-group-theory.md#translation-length) $\tau>0$. Nonzero powers have the same axis and

$$
\ell(a^m)=m\tau,
\qquad
\ell(a^n)=n\tau.
$$

Translation length is invariant under conjugacy, whereas the defining relation in the [Baumslag-Solitar group](../../../geometric-group-theory.md#baumslag-solitar-group) says that $a^m$ and $a^n$ are conjugate. Hence $m\tau=n\tau$, contradicting $m\ne n$. Therefore $a$ acts elliptically in every combinatorial tree action.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Suppose $G=A*B$ were a nontrivial [free product](../../../algebraic-topology.md#free-product). Its [Bass-Serre tree](../../../geometric-group-theory.md#bass-serre-tree) action has trivial edge stabilizers and no global fixed vertex. Part c makes $a$ elliptic. Since $a$ has infinite order, the fixed set of every nonzero power $a^r$ is a single vertex: it is nonempty, while fixing two vertices would fix the intervening edge and put the infinite-order element $a^r$ in a trivial edge stabilizer.

Let this vertex be $v$. The relation $ba^mb^{-1}=a^n$ gives

$$
b\operatorname{Fix}(a^m)=\operatorname{Fix}(a^n),
$$

and both sides are the singleton $\{v\}$. Thus $b$ also fixes $v$. Since $a$ and $b$ generate the [Baumslag-Solitar group](../../../geometric-group-theory.md#baumslag-solitar-group), the entire group fixes $v$, contradicting the Bass-Serre action of a nontrivial free product. Hence no such decomposition exists.

## 3

↑ **Parent:** [Paper 133](paper-133.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Any two [word metrics](../../../geometric-group-theory.md#word-metric) from finite generating sets on the same group are [bilipschitz equivalent](../../../geometric-group-theory.md#bilipschitz-equivalence). Indeed, if $S,S'$ are finite, let $L=\max_{s\in S}|s|_{S'}$; then $|g|_{S'}\leq L|g|_S$, and the reverse inequality follows symmetrically. Apply this once to the two finite generating sets of $G$ and once to those of $H$. Composing these bilipschitz identity maps with the inclusion changes only the multiplicative and additive constants in the [quasi-isometric embedding](../../../geometric-group-theory.md#quasi-isometric-embedding) inequalities. Thus being a [quasi-isometrically embedded subgroup](../../../geometric-group-theory.md#quasi-isometrically-embedded-subgroup) is independent of $S$ and $T$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $h\in H$ and let

$$
1=x_0,x_1,\ldots,x_N=h
$$

be a geodesic in the [Cayley graph](../../../geometric-group-theory.md#cayley-graph) $\operatorname{Cay}_S(G)$. By $K$-quasiconvexity choose $h_i\in H$ with $d_S(x_i,h_i)\leq K$, taking $h_0=1$ and $h_N=h$. Then

$$
|h_i^{-1}h_{i+1}|_S
\leq d_S(h_i,x_i)+1+d_S(x_{i+1},h_{i+1})
\leq2K+1.
$$

The elements $h_i^{-1}h_{i+1}$ telescope to $h$, so the finite set

$$
U=H\cap\{g:|g|_S\leq2K+1\}
$$

generates $H$.

Moreover $|h|_U\leq|h|_S$, while $|h|_S\leq(2K+1)|h|_U$. Thus the inclusion $(H,d_U)\to(G,d_S)$ is a [quasi-isometric embedding](../../../geometric-group-theory.md#quasi-isometric-embedding), and $H$ is quasi-isometrically embedded.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Take $G=\mathbb Z^2$ with the standard generating set $S=\{(1,0),(0,1)\}$, and let

$$
H=\langle(1,1)\rangle.
$$

Intrinsic distance in $H$ between $0$ and $(n,n)$ is $|n|$, while its ambient [word metric](../../../geometric-group-theory.md#word-metric) distance is $2|n|$, so $H$ is [quasi-isometrically embedded](../../../geometric-group-theory.md#quasi-isometrically-embedded-subgroup). However, the ambient geodesic from $(0,0)$ to $(n,n)$ that first travels to $(n,0)$ and then to $(n,n)$ contains $(n,0)$. Its distance from the diagonal subgroup $H$ is $n$. No uniform $K$ can contain every such geodesic in the $K$-neighborhood of $H$, so $H$ is not a [quasiconvex subgroup](../../../geometric-group-theory.md#quasiconvex-subgroup).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Choose a finite generating set $T$ of $H$. A $d_T$-geodesic between two elements of $H$ maps under the inclusion to a uniform [quasigeodesic](../../../geometric-group-theory.md#quasigeodesic) in $\operatorname{Cay}_S(G)$ because $H$ is quasi-isometrically embedded. Since $G$ is a [hyperbolic group](../../../geometric-group-theory.md#hyperbolic-group), the [Morse lemma for quasi-geodesics](../../../geometric-group-theory.md#morse-lemma-for-quasi-geodesics) gives a constant $R$ such that this quasigeodesic and the ambient geodesic with the same endpoints have Hausdorff distance at most $R$. Every vertex of the former lies in $H$, so the latter lies in the closed $R$-neighborhood of $H$. Therefore $H$ is a [quasiconvex subgroup](../../../geometric-group-theory.md#quasiconvex-subgroup).

## 4

↑ **Parent:** [Paper 133](paper-133.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $x,y\in X$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) and the fact that $\phi$ is an [isometry](../../../riemannian-geometry.md#isometry) give

$$
\begin{aligned}
|d_\phi(x)-d_\phi(y)|
&=|d(x,\phi x)-d(y,\phi y)|\\
&\leq d(x,y)+d(\phi x,\phi y)\\
&=2d(x,y).
\end{aligned}
$$

**Thus the [displacement function](../../../geometric-group-theory.md#displacement-function) is $2$-Lipschitz, hence [continuous](../../../calculus.md#continuous-function).**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Choose $y_n\in X$ with $d_\phi(y_n)\to0$. By the [cocompact group action](../../../geometric-group-theory.md#cocompact-group-action), there is a compact set $K\subseteq X$ whose translates cover $X$. Choose $\gamma_n\in\Gamma$ such that

$$
x_n:=\gamma_ny_n\in K,
\qquad
\phi_n:=\gamma_n\phi\gamma_n^{-1}.
$$

Isometric invariance gives

$$
d_{\phi_n}(x_n)
=d(\gamma_ny_n,\gamma_n\phi y_n)
=d_\phi(y_n)\longrightarrow0.
$$

For a fixed basepoint $x_0$, compactness of $K$ gives $C=\max_{x\in K}d(x_0,x)<\infty$, so $d(x_0,x_n)\leq C$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The bounded sequence $(x_n)$ lies in a compact set because $X$ is a [proper metric space](../../../geometric-group-theory.md#proper-metric-space). After taking a subsequence, $x_n\to x$. Since $d(x_n,\phi_nx_n)\to0$, both $x_n$ and $\phi_nx_n$ eventually lie in one compact neighborhood $L$ of $x$. A [properly discontinuous group action](../../../geometric-group-theory.md#properly-discontinuous-group-action) has only finitely many $g\in\Gamma$ with $gL\cap L\ne\varnothing$, so some conjugate $\psi$ occurs as $\phi_n$ along an infinite subsequence. Continuity then gives

$$
d(x,\psi x)=\lim_n d(x_n,\psi x_n)=0.
$$

**Thus $\psi$ fixes $x$. Since $\psi=\gamma\phi\gamma^{-1}$ for some $\gamma$, the original element $\phi$ fixes $\gamma^{-1}x$.**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Suppose a cocompact [Fuchsian group](../../../geometric-group-theory.md#fuchsian-group) contained a nonidentity [parabolic isometry of the hyperbolic plane](../../../geometric-group-theory.md#parabolic-isometry-of-the-hyperbolic-plane) $\phi$. After conjugating in the [upper half-plane model](../../../geometry-and-topology.md#poincare-half-plane-model), write $\phi(z)=z+c$ with $c\ne0$. The supplied estimate gives

$$
d(iy,\phi(iy))=d(iy,c+iy)\leq\frac{|c|}{y}\longrightarrow0
\qquad(y\to\infty),
$$

so the infimum of the displacement function is zero.

A Fuchsian action is properly discontinuous, and the action is cocompact by hypothesis. Parts b and c therefore imply that $\phi$ fixes a point of the [hyperbolic plane](../../../geometry-and-topology.md#hyperbolic-plane). A nonidentity parabolic isometry has no fixed point inside the plane, only one on its ideal boundary. This contradiction excludes nontrivial parabolic elements.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
