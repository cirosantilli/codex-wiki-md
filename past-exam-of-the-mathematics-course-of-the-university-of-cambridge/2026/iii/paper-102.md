# Paper 102

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20102%20updated.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20102%20updated.pdf)

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
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For this [Heisenberg Lie algebra](../../../lie-algebra.md#heisenberg-lie-algebra),

$$
[\mathfrak g,\mathfrak g]=\mathbb Cc,
\qquad
[\mathfrak g,\mathbb Cc]=0,
$$

because $c$ belongs to the [center](../../../lie-algebra.md#center-of-a-lie-algebra). Thus its [lower central series of a Lie algebra](../../../lie-algebra.md#lower-central-series-of-a-lie-algebra) is $\mathfrak g,\mathbb Cc,0$, so $\mathfrak g$ is a two-step [nilpotent Lie algebra](../../../lie-algebra.md#nilpotent-lie-algebra).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $A,B,C$ represent $a,b,c$. Since $c$ is central, $C$ commutes with $A$ and $B$. Over the [complex number](../../../complex-analysis.md#complex-number) field $\mathbb C$, $C$ has an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\gamma$, and its corresponding [eigenspace](../../../linear-operator-theory.md#eigenspace) is invariant under all three operators. The [irreducibility](../../../lie-algebra.md#irreducible-lie-algebra-representation) of $V$ therefore makes this eigenspace all of $V$, so $C=\gamma I$. Taking the [trace](../../../linear-algebra.md#matrix-trace) of

$$
C=[A,B]=AB-BA
$$

gives $(\dim V)\gamma=0$ by the [cyclic property of the trace](../../../linear-algebra.md#cyclic-property-of-the-trace); hence $C=0$.

The remaining operators $A$ and $B$ commute. Two commuting operators on a nonzero finite-dimensional complex [vector space](../../../vector-space.md) have a common [eigenvector](../../../linear-operator-theory.md#eigenvector), whose span is invariant. Irreducibility therefore forces $\dim V=1$. Conversely, every pair $(\alpha,\beta)\in\mathbb C^2$ defines a one-dimensional irreducible representation by

$$
a\longmapsto\alpha,
\qquad b\longmapsto\beta,
\qquad c\longmapsto0.
$$

These are all the finite-dimensional irreducible representations.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For a finite-dimensional [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) $\rho$ on $V$, the [Trace form of a Lie algebra representation](../../../lie-algebra.md#trace-form-of-a-lie-algebra-representation) is

$$
(x,y)_V=\operatorname{tr}\bigl(\rho(x)\rho(y)\bigr).
$$

Write again $A=\rho(a)$, $B=\rho(b)$, and $C=\rho(c)=[A,B]$. The operator $C$ commutes with both $A$ and $B$. Direct use of the [cyclic property of the trace](../../../linear-algebra.md#cyclic-property-of-the-trace) gives

$$
\begin{aligned}
\operatorname{tr}(CA)
&=\operatorname{tr}(ABA-BA^2)=0,\\
\operatorname{tr}(CB)
&=\operatorname{tr}(AB^2-BAB)=0,\\
\operatorname{tr}(C^2)
&=\operatorname{tr}(ABC-BAC)=0.
\end{aligned}
$$

In the last line, cyclicity and $AC=CA$ turn $\operatorname{tr}(ABC)$ into $\operatorname{tr}(BAC)$. Thus the nonzero vector $c\in\mathfrak g$ is orthogonal to the basis $a,b,c$, and hence to all of $\mathfrak g$. The [bilinear form](../../../linear-algebra.md#bilinear-form) is therefore [degenerate](../../../linear-algebra.md#degenerate-bilinear-form).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Use the [Polynomial representation of the Heisenberg Lie algebra](../../../lie-algebra.md#polynomial-representation-of-the-heisenberg-lie-algebra) on the infinite-dimensional [polynomial ring](../../../commutative-algebra.md#polynomial-ring) $\mathbb C[x]$:

$$
a\cdot f=f',
\qquad b\cdot f=xf,
\qquad c\cdot f=f.
$$

The [product rule](../../../calculus.md#product-rule) gives $[d/dx,x]=1$, so this is a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation). It is a [Faithful Lie algebra representation](../../../lie-algebra.md#faithful-lie-algebra-representation): if $\alpha(d/dx)+\beta x+\gamma$ is the zero operator, applying it first to $1$ gives $\beta x+\gamma=0$, and then applying the remaining operator to $x$ gives $\alpha=0$.

To prove [irreducibility](../../../lie-algebra.md#irreducible-lie-algebra-representation), let $W$ be a nonzero invariant [subspace](../../../vector-space.md#vector-subspace) and choose a nonzero polynomial in $W$ of least degree. If its degree were positive, repeated [differentiation](../../../calculus.md#derivative) would produce a nonzero element of smaller degree, so $W$ contains a nonzero constant. Invariance under multiplication by $x$ then puts every monomial $x^n$ in $W$, and hence $W=\mathbb C[x]$.

## 2

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Choose the [Borel subalgebra](../../../semisimple-lie-algebra.md#borel-subalgebra) $\mathfrak b=\mathfrak t\oplus\mathfrak n^+$ determined by the positive roots. Regard the one-dimensional space $\mathbb C_\lambda$ as a $\mathfrak b$-module on which $\mathfrak n^+$ acts by zero and $h\in\mathfrak t$ acts by $\lambda(h)$. The [Verma module](../../../semisimple-lie-algebra.md#verma-module) is

$$
M_\lambda=U(\mathfrak g)\otimes_{U(\mathfrak b)}\mathbb C_\lambda.
$$

The [Poincaré-Birkhoff-Witt theorem](../../../lie-algebra.md#poincare-birkhoff-witt-theorem) identifies it as a vector space with $U(\mathfrak n^-)$ acting on a highest-weight vector $v_\lambda$.

For each positive root $\alpha$, arbitrary powers of a negative-root vector contribute the geometric series $1+e^{-\alpha}+e^{-2\alpha}+\cdots$. Consequently the [formal character of a weight module](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module) is

$$
\operatorname{ch}M_\lambda
=e^\lambda\prod_{\alpha\in R^+}(1-e^{-\alpha})^{-1}.
$$

This product is interpreted in the completion of the group algebra in the negative-root direction; the PBW basis proves that every coefficient is the correct finite [weight space](../../../semisimple-lie-algebra.md#weight-space) dimension.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [weights](../../../semisimple-lie-algebra.md#weight-of-a-representation) of $M_\lambda$ lie below $\lambda$ in the positive-root order, and every [weight space](../../../semisimple-lie-algebra.md#weight-space) is finite-dimensional. A nonzero submodule $V$ is stable under the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra), so it is a direct sum of its weight spaces. Choose a maximal weight $\mu$ occurring in $V$. Every positive-root operator would raise its weight; maximality therefore makes it kill any nonzero $v\in V_\mu$. Thus $v$ is a [singular vector](../../../semisimple-lie-algebra.md#singular-vector).

The [Casimir element](../../../semisimple-lie-algebra.md#casimir-element) is central and acts throughout $M_\lambda$ by

$$
|\lambda+\rho|^2-|\rho|^2.
$$

The same element acts on the highest-weight vector $v$ of weight $\mu$ by

$$
|\mu+\rho|^2-|\rho|^2.
$$

Both are the action of one operator on the same module, so the scalars agree and

$$
\boxed{|\mu+\rho|=|\lambda+\rho|.}
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

For the [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra), let $v_\lambda$ be the highest-weight vector. The [Poincaré-Birkhoff-Witt theorem](../../../lie-algebra.md#poincare-birkhoff-witt-theorem) gives the basis $(f^rv_\lambda)_{r\geq0}$, and the defining [Lie brackets](../../../lie-algebra.md#lie-bracket) imply

$$
e f^rv_\lambda=r(\lambda-r+1)f^{r-1}v_\lambda.
$$

A positive-degree basis vector is [singular](../../../semisimple-lie-algebra.md#singular-vector) exactly when $r=\lambda+1$ is a positive integer. Therefore $M_\lambda$ is irreducible when $\lambda\notin\mathbb Z_{\geq0}$.

If $\lambda=m\in\mathbb Z_{\geq0}$, the vector $f^{m+1}v_\lambda$ has weight $-m-2$ and generates a submodule isomorphic to $M_{-m-2}$. The latter is irreducible because $-m-2\notin\mathbb Z_{\geq0}$. Every nonzero submodule contains a [singular vector](../../../semisimple-lie-algebra.md#singular-vector) by the preceding part, and the displayed coefficient shows that this is the only possible proper singular vector. Hence

$$
U(\mathfrak{sl}_2)f^{m+1}v_\lambda\cong M_{-m-2}
$$

is the unique proper nonzero submodule, as summarized by the [Reducibility of an sl2 Verma module](../../../semisimple-lie-algebra.md#reducibility-of-an-sl2-verma-module).

## 3

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

After ordering a [symplectic basis](../../../linear-algebra.md#symplectic-basis) in two blocks, write

$$
h=\operatorname{diag}(t_1,\ldots,t_n,-t_1,\ldots,-t_n),
\qquad \varepsilon_i(h)=t_i.
$$

Matrices in the [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra) have block form

$$
\begin{pmatrix}A&B\\ C&-A^T\end{pmatrix},
\qquad B=B^T,quad C=C^T.
$$

The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) is

$$
\mathfrak{sp}_{2n}=\mathfrak t
\oplus\bigoplus_{i\ne j}\mathfrak g_{\varepsilon_i-\varepsilon_j}
\oplus\bigoplus_{i<j}\left(\mathfrak g_{\varepsilon_i+\varepsilon_j}\oplus\mathfrak g_{-\varepsilon_i-\varepsilon_j}\right)
\oplus\bigoplus_i\left(\mathfrak g_{2\varepsilon_i}\oplus\mathfrak g_{-2\varepsilon_i}\right).
$$

For example, these one-dimensional spaces are spanned respectively by

$$
E_{ij}-E_{n+j,n+i},\quad
E_{i,n+j}+E_{j,n+i},\quad
E_{n+i,j}+E_{n+j,i},\quad
E_{i,n+i},\quad E_{n+i,i}.
$$

Thus this is the [Cn root system](../../../semisimple-lie-algebra.md#cn-root-system)

$$
R=\{\pm\varepsilon_i\pm\varepsilon_j:i<j\}\cup\{\pm2\varepsilon_i:1\leq i\leq n\}.
$$

The upper-triangular choice gives

$$
R^+=\{\varepsilon_i-\varepsilon_j:i<j\}
\cup\{\varepsilon_i+\varepsilon_j:i<j\}
\cup\{2\varepsilon_i:1\leq i\leq n\}.
$$

Its [simple roots](../../../semisimple-lie-algebra.md#simple-root), [highest root](../../../semisimple-lie-algebra.md#highest-root), [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight), and [half-sum of positive roots](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots) are

$$
\begin{aligned}
\alpha_i&=\varepsilon_i-\varepsilon_{i+1} &&(1\leq i<n),&
\alpha_n&=2\varepsilon_n,\\
\theta&=2\varepsilon_1,&
\omega_k&=\varepsilon_1+\cdots+\varepsilon_k &&(1\leq k\leq n),\\
\rho&=n\varepsilon_1+(n-1)\varepsilon_2+\cdots+\varepsilon_n.
\end{aligned}
$$

Using the notation requested in the paper, the root lattice $P$ and weight lattice $Q$ are

$$
P=\left\{(m_1,\ldots,m_n)\in\mathbb Z^n:\sum_i m_i\equiv0\pmod2\right\},
\qquad Q=\mathbb Z^n,
$$

so $Q/P\cong\mathbb Z/2\mathbb Z$. This reverses the common notation in which the [root lattice](../../../semisimple-lie-algebra.md#root-lattice) is called $Q$ and the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) is called $P$.

Since a multiple-edge arrow in a [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) points toward the shorter root, the finite and [extended](../../../semisimple-lie-algebra.md#extended-dynkin-diagram) diagrams are

$$
\alpha_1-\alpha_2-\cdots-\alpha_{n-2}-\alpha_{n-1}\Longleftarrow\alpha_n
$$

and

$$
\alpha_0\Longrightarrow\alpha_1-\alpha_2-\cdots-\alpha_{n-2}-\alpha_{n-1}\Longleftarrow\alpha_n,
\qquad \alpha_0=-2\varepsilon_1.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) formula $s_\alpha(x)=x-\langle x,\alpha^\vee\rangle\alpha$ becomes especially concrete on $x=(x_1,\ldots,x_n)$:

$$
\begin{aligned}
s_{\varepsilon_i-\varepsilon_j}&:\ (x_i,x_j)\longmapsto(x_j,x_i),\\
s_{\varepsilon_i+\varepsilon_j}&:\ (x_i,x_j)\longmapsto(-x_j,-x_i),\\
s_{2\varepsilon_i}&:\ x_i\longmapsto-x_i,
\end{aligned}
$$

with all unlisted coordinates fixed. The [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is therefore the group of signed permutations

$$
\boxed{W\cong(\mathbb Z/2\mathbb Z)^n\rtimes S_n.}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

With

$$
J=\begin{pmatrix}0&1\\-1&0\end{pmatrix},
\qquad
A=\begin{pmatrix}p&q\\r&s\end{pmatrix},
$$

the equation $AJ+JA^T=0$ reduces to $p+s=0$. Hence

$$
\mathfrak{sp}_2
=\left\{\begin{pmatrix}p&q\\r&-p\end{pmatrix}:p,q,r\in\mathbb C\right\}
=\mathfrak{sl}_2
$$

as matrix [Lie algebras](../../../lie-algebra.md), with the same [commutator](../../../lie-algebra.md#commutator) bracket.

## 4

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Let $R^+$ be the [positive roots](../../../semisimple-lie-algebra.md#positive-root), $W$ the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group), $\ell(w)$ its [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length), $\rho$ the [half-sum of positive roots](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots), and $\alpha^\vee$ a [coroot](../../../semisimple-lie-algebra.md#coroot). For a dominant integral highest weight $\lambda$, the [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula) is

$$
\operatorname{ch}L_\lambda
=\frac{\sum_{w\in W}(-1)^{\ell(w)}e^{w(\lambda+\rho)}}
{\sum_{w\in W}(-1)^{\ell(w)}e^{w\rho}}
=\frac{\sum_{w\in W}(-1)^{\ell(w)}e^{w(\lambda+\rho)}}
{e^\rho\prod_{\alpha\in R^+}(1-e^{-\alpha})}.
$$

Taking the value at the identity gives the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula)

$$
\dim L_\lambda
=\prod_{\alpha\in R^+}
\frac{\langle\lambda+\rho,\alpha^\vee\rangle}
{\langle\rho,\alpha^\vee\rangle}.
$$

For the q-character convention relevant to the [Principal sl2 subalgebra](../../../semisimple-lie-algebra.md#principal-sl2-subalgebra), set $h_{\mathrm{pr}}=2\rho^\vee$, so $\alpha_i(h_{\mathrm{pr}})=2$ for every simple root, and define

$$
\operatorname{ch}_qL_\lambda
=\sum_\mu(\dim L_\lambda[\mu])q^{\mu(h_{\mathrm{pr}})}.
$$

The q-character formula is the principal specialization of the [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula):

$$
\boxed{\operatorname{ch}_qL_\lambda
=\frac{\sum_{w\in W}(-1)^{\ell(w)}q^{\langle w(\lambda+\rho),2\rho^\vee\rangle}}
{\sum_{w\in W}(-1)^{\ell(w)}q^{\langle w\rho,2\rho^\vee\rangle}}.}
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Choose a short simple root $\alpha_1$ and a long simple root $\alpha_2$, with $|\alpha_2|^2=3|\alpha_1|^2$ and angle $150^\circ$. The six positive roots of the [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system) are

$$
\alpha_1,\ \alpha_2,\ \alpha_1+\alpha_2,\ 2\alpha_1+\alpha_2,\ 3\alpha_1+\alpha_2,\ 3\alpha_1+2\alpha_2,
$$

and their negatives complete the two concentric hexagons of short and long roots. The [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) are

$$
\omega_1=2\alpha_1+\alpha_2,
\qquad
\omega_2=3\alpha_1+2\alpha_2,
$$

so $\omega_1$ is itself a short root and $\omega_2$ is the [highest root](../../../semisimple-lie-algebra.md#highest-root).

The seven-dimensional representation $L_{\omega_1}$ has weight set

$$
0,\quad
\pm\alpha_1,\quad
\pm(\alpha_1+\alpha_2),\quad
\pm(2\alpha_1+\alpha_2),
$$

each with [weight multiplicity](../../../semisimple-lie-algebra.md#weight-multiplicity) one. Their positive heights are $1,2,3$, so the [q-character of a highest-weight representation](../../../semisimple-lie-algebra.md#q-character-of-a-highest-weight-representation) is

$$
\operatorname{ch}_qL_{\omega_1}
=q^6+q^4+q^2+1+q^{-2}+q^{-4}+q^{-6}.
$$

This is one $\mathfrak{sl}_2$ weight string, hence

$$
L_{\omega_1}\downarrow\mathfrak{sl}_2^{\mathrm{pr}}\cong V_6.
$$

The representation $L_{\omega_2}$ is the fourteen-dimensional [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). Its nonzero weights are the twelve roots, and its zero-weight space is the two-dimensional [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra). The positive root heights are $1,1,2,3,4,5$, so

$$
\begin{aligned}
\operatorname{ch}_qL_{\omega_2}
={}&q^{10}+q^8+q^6+q^4+2q^2+2\\
&+2q^{-2}+q^{-4}+q^{-6}+q^{-8}+q^{-10}.
\end{aligned}
$$

Splitting this into ordinary $\mathfrak{sl}_2$ strings gives

$$
\boxed{L_{\omega_2}\downarrow\mathfrak{sl}_2^{\mathrm{pr}}
\cong V_{10}\oplus V_2.}
$$

## 5

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use the [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system) convention

$$
\alpha_1=\varepsilon_2,
\qquad
\alpha_2=\varepsilon_1-\varepsilon_2,
\qquad
\omega_1=\frac{\varepsilon_1+\varepsilon_2}{2},
\qquad
\omega_2=\varepsilon_1.
$$

Thus $V=L_{\omega_2}$ is the five-dimensional vector representation of the [Special orthogonal Lie algebra](../../../semisimple-lie-algebra.md#special-orthogonal-lie-algebra) $\mathfrak{so}_5$. Label its weight vertices

$$
A=\varepsilon_1,quad B=\varepsilon_2,quad C=0,quad D=-\varepsilon_2,quad E=-\varepsilon_1.
$$

The [crystal basis](../../../semisimple-lie-algebra.md#crystal-basis) is the colored chain

$$
A\xrightarrow{2}B\xrightarrow{1}C\xrightarrow{1}D\xrightarrow{2}E,
$$

because each [Kashiwara operator](../../../semisimple-lie-algebra.md#kashiwara-operator) $\widetilde f_i$ subtracts $\alpha_i$.

For the [tensor product of crystals](../../../semisimple-lie-algebra.md#tensor-product-of-crystals), write $XY$ for $X\otimes Y$. The complete colored-arrow graph is compactly specified by

$$
\begin{aligned}
\text{color }1:\quad&
AB\to AC\to AD,\quad BA\to CA\to DA,\quad
BB\to CB\to DB\to DC\to DD,\\
&BC\to CC\to CD,\quad BE\to CE\to DE,\quad EB\to EC\to ED;\\
\text{color }2:\quad&
AA\to BA\to BB,\quad AC\to BC,\quad AD\to BD\to BE,\\
&CA\to CB,\quad CD\to CE,\quad DA\to EA\to EB,\quad
DC\to EC,\quad DD\to ED\to EE.
\end{aligned}
$$

Its three connected highest-weight components start at $AA$, $AB$, and $AE$. Their vertex sets are

$$
\begin{aligned}
B(2\omega_2):\quad&AA,BA,BB,CA,CB,DA,DB,DC,DD,EA,EB,EC,ED,EE,\\
B(2\omega_1):\quad&AB,AC,AD,BC,BD,BE,CC,CD,CE,DE,\\
B(0):\quad&AE.
\end{aligned}
$$

Their highest weights and dimensions identify the ten-vertex component with the [exterior square](../../../linear-algebra.md#exterior-square) and the other two with the [symmetric square](../../../linear-algebra.md#symmetric-square). Therefore

$$
\bigwedge^2V\cong L_{2\omega_1},
\qquad
S^2V\cong L_{2\omega_2}\oplus L_0,
$$

of dimensions $10$ and $14+1$, respectively.

The module $L=L_{\omega_1}$ is the four-dimensional spin representation. Its weights are $(\pm\varepsilon_1\pm\varepsilon_2)/2$, and its crystal is

$$
\frac{\varepsilon_1+\varepsilon_2}{2}
\xrightarrow{1}
\frac{\varepsilon_1-\varepsilon_2}{2}
\xrightarrow{2}
\frac{-\varepsilon_1+\varepsilon_2}{2}
\xrightarrow{1}
\frac{-\varepsilon_1-\varepsilon_2}{2}.
$$

Every weight of $V$ lies in the [root lattice](../../../semisimple-lie-algebra.md#root-lattice), so every weight of every [tensor power](../../../linear-algebra.md#tensor-power) $V^{\otimes n}$ also lies in that lattice. But $\omega_1=(\varepsilon_1+\varepsilon_2)/2$ represents the nonzero coset in the quotient of the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) by the root lattice. Consequently no irreducible constituent of $V^{\otimes n}$ can have highest weight $\omega_1$, and $L$ never occurs.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
