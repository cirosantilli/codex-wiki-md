# Paper 4

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper4.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper4.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
  - [v](#4/v)
    - [Solution](#4/v/solution)
  - [vi](#4/vi)
    - [Solution](#4/vi/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)

## 1

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Take $B$ to be linear in its first argument and conjugate-linear in its second, with $\bar a=a^q$. For a [Hermitian form over a quadratic finite field](../../../linear-algebra.md#hermitian-form-over-a-quadratic-finite-field), $B(v,v)\in\mathbb F_q$. We first establish the [quadratic finite-field norm and trace surjectivity](../../../algebra.md#quadratic-finite-field-norm-and-trace-surjectivity) needed for [orthonormalization of a finite-field Hermitian form](../../../linear-algebra.md#orthonormalization-of-a-finite-field-hermitian-form). The [field norm](../../../algebraic-number-theory.md#field-norm) $N(a)=a^{q+1}$ maps $\mathbb F_{q^2}^*$ onto $\mathbb F_q^*$ because the [multiplicative group of a finite field is cyclic](../../../algebra.md#multiplicative-group-of-a-finite-field-is-cyclic) of order $q^2-1$. The [field trace](../../../algebraic-number-theory.md#field-trace) $\operatorname{Tr}(a)=a+a^q$ is an $\mathbb F_q$-linear map into $\mathbb F_q$. It is nonzero: a nonzero polynomial of degree $q$ cannot vanish at all $q^2$ elements. It is therefore onto, including in characteristic two.

There must be $v$ with $B(v,v)\ne0$. Otherwise, for any $v,w,a$, expanding the diagonal value gives

$$
0=B(v+aw,v+aw)=\operatorname{Tr}(\bar a B(v,w)).
$$

If $B(v,w)\ne0$, varying $a$ contradicts the surjectivity of the [field trace](../../../algebraic-number-theory.md#field-trace). Thus all pairings would vanish, contrary to nondegeneracy. Choose $a$ with $N(a)=B(v,v)^{-1}$; then $v_1=av$ has norm one. Every $w$ decomposes uniquely as

$$
w=B(w,v_1)v_1+\bigl(w-B(w,v_1)v_1\bigr),\qquad V=\mathbb F_{q^2}v_1\oplus v_1^\perp.
$$

The restricted [Hermitian form over a quadratic finite field](../../../linear-algebra.md#hermitian-form-over-a-quadratic-finite-field) on the [orthogonal complement for a sesquilinear form](../../../linear-algebra.md#orthogonal-complement-for-a-sesquilinear-form) is nondegenerate: a vector there orthogonal to that complement is also orthogonal to $v_1$, hence to all of $V$, and is zero. Induction produces an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $v_1,\ldots,v_n$.

The [unitary group over a finite field](../../../finite-group-theory.md#unitary-group-over-a-finite-field) is the [group](../../../group.md) of invertible $\mathbb F_{q^2}$-linear maps preserving $B$. In the [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) just constructed, its concise description is

$$
\boxed{U_n(q^2)=\{g\in GL_n(\mathbb F_{q^2}):\bar g^{\mathsf T}g=I_n\}.}
$$

The notation here uses the size of the matrix field; it is also frequently written $U_n(q)$. There is no determinant-one condition in this definition.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

We construct a [Hermitian hyperbolic plane over a finite field](../../../linear-algebra.md#hermitian-hyperbolic-plane-over-a-finite-field) inside each successive two-dimensional piece. By the [field norm](../../../algebraic-number-theory.md#field-norm) surjectivity proved above, choose $a\in\mathbb F_{q^2}$ with $a\bar a=-1$. From two vectors in an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), form $e=v_1+av_2$. Then $B(e,e)=1+a\bar a=0$, so $e$ is a nonzero [isotropic vector](../../../linear-algebra.md#isotropic-vector). Nondegeneracy supplies $g$ with $B(e,g)=1$; rescaling the second argument achieves this normalization. In fact $g=v_1$ already works in this two-dimensional piece. By [quadratic finite-field norm and trace surjectivity](../../../algebra.md#quadratic-finite-field-norm-and-trace-surjectivity), choose $c$ with $c+\bar c=B(g,g)$ and put $f=g-ce$. Direct expansion gives

$$
B(e,f)=1,\qquad B(f,f)=B(g,g)-c-\bar c=0.
$$

Thus $e,f$ are [linearly independent](../../../vector-space.md#linear-independence), and their [Gram matrix](../../../linear-algebra.md#gram-matrix) is $\begin{pmatrix}0&1\\1&0\end{pmatrix}$, which is invertible even in characteristic two. Their span is nondegenerate, so its [orthogonal complement for a sesquilinear form](../../../linear-algebra.md#orthogonal-complement-for-a-sesquilinear-form) is again nondegenerate. Repeat the construction there. In even dimension this exhausts $V$; in odd dimension the final one-dimensional complement has a nonzero diagonal value, which can be normalized to one using the [field norm](../../../algebraic-number-theory.md#field-norm). Calling its vector $d$, we obtain

$$
\boxed{B(e_i,f_j)=\delta_{ij},\quad B(e_i,e_j)=B(f_i,f_j)=0,\quad B(d,d)=1,\quad B(d,e_i)=B(d,f_i)=0,}
$$

with the $d$ terms present only in odd dimension. This proves all the requested pairings and the [basis](../../../vector-space.md#basis) assertion.

The printed hint needs a qualification. If $X^2-X-1$ is irreducible over $\mathbb F_q$, its two roots are conjugate, so $\zeta+\bar\zeta=1$ and $\zeta\bar\zeta=-1$; the hinted vectors then do work. They need not work when it splits. For example, over $\mathbb F_{11}$ its roots are $4,8$, fixed by conjugation in $\mathbb F_{121}$. For either choice the proposed $e$ has norm $1+\zeta^2$, respectively $6$ or $10$, rather than zero. The norm-and-trace construction above proves the assertion without that restriction.

## 2

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use the course convention that a [root system](../../../semisimple-lie-algebra.md#root-system) is finite and is a [reduced root system](../../../semisimple-lie-algebra.md#reduced-root-system) satisfying the [crystallographic root system](../../../semisimple-lie-algebra.md#crystallographic-root-system) condition. These hypotheses are essential for the angle restriction. For [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) $r,s$, the two [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer)

$$
a=\frac{2(r,s)}{(s,s)},\qquad b=\frac{2(r,s)}{(r,r)}
$$

satisfy $ab=4\cos^2\theta$. If $r,s$ are not parallel, the strict [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and integrality give $ab\in\{0,1,2,3\}$. These values give angles $\pi/2$, $\pi/3$ or $2\pi/3$, $\pi/4$ or $3\pi/4$, and $\pi/6$ or $5\pi/6$, respectively. If the roots are parallel, reducedness implies $s=\pm r$, giving $0$ or $\pi$. Therefore

$$
\boxed{\theta\in\{0,\pi/6,\pi/4,\pi/3,\pi/2,2\pi/3,3\pi/4,5\pi/6,\pi\}.}
$$

Here are examples accounting for every angle. In the [A1 root system](../../../semisimple-lie-algebra.md#rank-one-root-system), the pairs $(r,r)$ and $(r,-r)$ give $0,\pi$. Two roots from different summands of $A_1\oplus A_1$ give $\pi/2$. The six unit vectors at angles $k\pi/3$ form an [A2 root system](../../../semisimple-lie-algebra.md#a2-root-system): taking one root at angle zero and another at $\pi/3$ or $2\pi/3$ gives those two angles. In the [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system) $\{\pm e_1,\pm e_2,\pm e_1\pm e_2\}$, pair $e_1$ with $e_1+e_2$ or $-e_1+e_2$ to obtain $\pi/4,3\pi/4$. In a [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system), take short unit roots at angles $k\pi/3$ and long roots of length $\sqrt3$ at angles $\pi/6+k\pi/3$. A short root at zero paired with long roots at $\pi/6,5\pi/6$ gives the remaining angles.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

If the [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) are parallel, their [Euclidean norms](../../../functional-analysis.md#euclidean-norm) are equal by reducedness. For nonparallel, nonorthogonal roots, the [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer) $a,b$ above are nonzero integers of the same sign and have product $1,2$ or $3$. Also

$$
\frac{(r,r)}{(s,s)}=\frac{a}{b}.
$$

The absolute pairs $(|a|,|b|)$ are $(1,1)$, $(1,2),(2,1)$, or $(1,3),(3,1)$. Hence

$$
\boxed{\frac{\|r\|}{\|s\|}\in\{1,\sqrt2,1/\sqrt2,\sqrt3,1/\sqrt3\}.}
$$

More precisely, angles $\pi/3,2\pi/3$ require equal lengths; angles $\pi/4,3\pi/4$ require a long-to-short ratio $\sqrt2$; and angles $\pi/6,5\pi/6$ require a ratio $\sqrt3$. The exclusion of orthogonality matters: orthogonal irreducible components can be scaled independently.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Choose a [fundamental system of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) $\{\alpha,\beta\}$. Distinct [simple roots](../../../semisimple-lie-algebra.md#simple-root) have nonpositive inner product. Their [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) has diagonal entries two and off-diagonal entries $-p,-q$, where either $p=q=0$, or $p,q$ are positive integers. The [root-system finiteness lemma](../../../semisimple-lie-algebra.md#root-system-finiteness-lemma) gives $pq<4$. After exchanging the simple roots, the possibilities are

$$
\begin{pmatrix}2&0\\0&2\end{pmatrix},\quad
\begin{pmatrix}2&-1\\-1&2\end{pmatrix},\quad
\begin{pmatrix}2&-1\\-2&2\end{pmatrix},\quad
\begin{pmatrix}2&-1\\-3&2\end{pmatrix}.
$$

Their angles and relative lengths determine the two simple roots up to an orthogonal transformation and common scaling, except that the two orthogonal components can be scaled separately.

To see that no extra roots remain unspecified, write a positive root $\gamma=m\alpha+n\beta$ with nonnegative integer coefficients. If it is not simple, some simple root $\delta$ has $(\gamma,\delta)>0$: otherwise $\|\gamma\|^2=m(\gamma,\alpha)+n(\gamma,\beta)\le0$. The [root reflection](../../../semisimple-lie-algebra.md#root-reflection) in $\delta$ subtracts a positive integer multiple of $\delta$. The other coordinate stays nonnegative; since $\gamma$ is not proportional to $\delta$, it is positive, so the reflected root must still be positive by the defining sign property of a [fundamental system of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system). Its height decreases. Repeating reduces $\gamma$ to a simple root. Thus every root is in a [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) orbit of a simple root.

For the four matrices, applying their simple reflections gives, respectively, the following positive roots:

$$
\begin{array}{c|l}
A_1\oplus A_1&\alpha,\beta\\
A_2&\alpha,\beta,\alpha+\beta\\
B_2&\alpha,\beta,\alpha+\beta,\alpha+2\beta\\
G_2&\alpha,\beta,\alpha+\beta,\alpha+2\beta,\alpha+3\beta,2\alpha+3\beta
\end{array}
$$

where in the last two rows $\alpha$ is long, $\beta$ short. For example, $s_\beta(\alpha)=\alpha+q\beta$ and $s_\alpha(\beta)=\beta+\alpha$ for the displayed matrices when the convention is $a_{ij}=2(\alpha_i,\alpha_j)/(\alpha_i,\alpha_i)$. The sets comprising these positive roots and their negatives are invariant under both reflections, as direct substitution verifies. The height argument therefore shows they are the whole [root system](../../../semisimple-lie-algebra.md#root-system). This proves the [classification of rank-two root systems](../../../semisimple-lie-algebra.md#classification-of-rank-two-root-systems):

$$
\boxed{A_1\oplus A_1,\quad A_2,\quad B_2,\quad G_2.}
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

A [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) has one vertex for each [simple root](../../../semisimple-lie-algebra.md#simple-root). Vertices $i,j$ are joined by $a_{ij}a_{ji}$ bonds, where $a_{ij}$ are the off-diagonal [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer). No bond means orthogonality; one, two and three bonds mean angles $2\pi/3,3\pi/4,5\pi/6$. A multiple-bond arrow points to the shorter root. Thus the [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) determines the [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix), including the relative lengths inside each connected component.

An [irreducible root system](../../../semisimple-lie-algebra.md#irreducible-root-system) corresponds to a connected [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram). The [classification of finite crystallographic Dynkin diagrams](../../../semisimple-lie-algebra.md#classification-of-finite-crystallographic-dynkin-diagrams) gives

$$
\boxed{A_l\ (l\ge1),\ B_l\ (l\ge2),\ C_l\ (l\ge3),\ D_l\ (l\ge4),\ E_6,E_7,E_8,F_4,G_2.}
$$

Here $C_2$ is already represented by $B_2$, and $B_1,C_1$ by $A_1$. General systems are orthogonal direct sums of these, with separate component scales. The following diagrams specify all the types; dots denote a continued chain, not additional vertices.

<a id="2/iv/image-finite-irreducible-crystallographic-dynkin-diagrams-with-every-arrow-pointing-toward-the-shorter-root"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-4-dynkin-diagrams.png)

**[Figure 1](#2/iv/image-finite-irreducible-crystallographic-dynkin-diagrams-with-every-arrow-pointing-toward-the-shorter-root). Finite irreducible crystallographic Dynkin diagrams, with every arrow pointing toward the shorter root**.

For orientation, the [An Dynkin diagram](../../../semisimple-lie-algebra.md#an-dynkin-diagram) is a single chain, the [Bn Dynkin diagram](../../../semisimple-lie-algebra.md#bn-dynkin-diagram-and-affine-extension) has a terminal double bond pointing to its terminal short root, and the [Cn Dynkin diagram](../../../semisimple-lie-algebra.md#cn-dynkin-diagram) reverses that arrow. The [Dn Dynkin diagram](../../../semisimple-lie-algebra.md#dn-dynkin-diagram) has arm lengths $1,1,l-3$. The [En Dynkin diagram](../../../semisimple-lie-algebra.md#en-dynkin-diagram) has arm lengths $1,2,2$; $1,2,3$; or $1,2,4$. The [F4 Dynkin diagram](../../../semisimple-lie-algebra.md#f4-dynkin-diagram) has a central double bond and the [G2 Dynkin diagram](../../../semisimple-lie-algebra.md#g2-dynkin-diagram) a triple bond.

The positivity behind this finite list is the positive-definite Gram matrix of the [simple roots](../../../semisimple-lie-algebra.md#simple-root). In particular the underlying graph is a tree: if it contained a cycle, the sum of its normalized roots would have squared norm at most zero, since each bonded inner product is at most $-1/2$. This contradicts [linear independence](../../../vector-space.md#linear-independence). Restricting the possible bonds and branches by positive definiteness gives precisely the listed chains and trees. Conversely their [Cartan matrices](../../../semisimple-lie-algebra.md#cartan-matrix) are positive definite after symmetrization and their reflection-generated root sets give the indicated finite [root systems](../../../semisimple-lie-algebra.md#root-system).

## 3

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Put $u(t)=\begin{pmatrix}1&t\\0&1\end{pmatrix}$ and $l(s)=\begin{pmatrix}1&0\\s&1\end{pmatrix}$. These [elementary matrices](../../../numerical-analysis.md#elementary-matrix) belong to the [special linear group](../../../group-theory.md#special-linear-group). Let $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ have determinant one. If $a\ne0$, elementary row elimination gives

$$
l(-c/a)g=\begin{pmatrix}a&b\\0&a^{-1}\end{pmatrix}
=\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}u(b/a).
$$

The remaining diagonal matrix is also a product of the given generators. Indeed, for $a\ne0$, direct multiplication gives

$$
w(a):=u(a)l(-a^{-1})u(a)=\begin{pmatrix}0&a\\-a^{-1}&0\end{pmatrix},\qquad
w(a)w(-1)=\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}.
$$

Hence $g=l(c/a)w(a)w(-1)u(b/a)$. If $a=0$, its [determinant](../../../linear-algebra.md#determinant) forces $c\ne0$, and $u(1)g$ has upper-left entry $c$. The established case applies to it, and $g=u(-1)(u(1)g)$ is again generated. No division by two was used, so the proof works over every [field](../../../algebra.md#field). **The upper and lower elementary unipotent matrices generate $SL_2(K)$.**

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Here $A_1(K)$ denotes the [adjoint Chevalley group of type A1](../../../lie-theory.md#adjoint-chevalley-group-of-type-a1); the isogeny form matters, since the simply connected form is $SL_2(K)$ itself. Over $\mathbb C$, take the [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) with [Chevalley basis](../../../semisimple-lie-algebra.md#chevalley-basis)

$$
e=\begin{pmatrix}0&1\\0&0\end{pmatrix},\quad
f=\begin{pmatrix}0&0\\1&0\end{pmatrix},\quad
h=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

Their [Lie brackets](../../../lie-algebra.md#lie-bracket) satisfy $[h,e]=2e$, $[h,f]=-2f$, $[e,f]=h$. Conjugation defines a [group homomorphism](../../../group-theory.md#group-homomorphism) $\rho:SL_2(\mathbb C)\to\operatorname{Aut}(\mathfrak{sl}_2(\mathbb C))$. Since $e^2=f^2=0$, $u(t)=\exp(te)$ and $l(s)=\exp(sf)$. Differentiating conjugation, or expanding its finite polynomial on this basis, gives

$$
\rho(u(t))=\exp(t\operatorname{ad}e),\qquad
\rho(l(s))=\exp(s\operatorname{ad}f).
$$

The [adjoint Chevalley group](../../../lie-theory.md#adjoint-chevalley-group) is generated by these two families. Part (i) therefore proves that it is exactly the image of $\rho$. A matrix commuting with $e$ has the form $\begin{pmatrix}a&b\\0&a\end{pmatrix}$; also commuting with $f$ forces $b=0$. Thus the [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) $\ker\rho$ consists of scalar matrices of determinant one, namely $\{I,-I\}$. The [first isomorphism theorem](../../../group-theory.md#first-isomorphism-theorem) now gives $A_1(\mathbb C)\cong SL_2(\mathbb C)/\{\pm I\}=PSL_2(\mathbb C)$.

For a general [field](../../../algebra.md#field), first compute the [Chevalley basis](../../../semisimple-lie-algebra.md#chevalley-basis) root operators as integral polynomials, and only then reduce their coefficients to $K$. Explicitly,

$$
\begin{aligned}
x_+(t)e&=e,&x_+(t)h&=h-2te,&x_+(t)f&=f+th-t^2e,\\
x_-(s)f&=f,&x_-(s)h&=h+2sf,&x_-(s)e&=e-sh-s^2f.
\end{aligned}
$$

They are still precisely conjugation by $u(t),l(s)$ on the three-dimensional trace-zero matrix space. These formulas remain valid in characteristic two, where $h=I$ but $e,h,f$ remain [linearly independent](../../../vector-space.md#linear-independence). Part (i) still identifies the generated image with the conjugation image of $SL_2(K)$. The same computation with $e,f$ gives [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) $\{aI:a^2=1\}$, exactly its scalar center. Consequently

$$
\boxed{A_1(K)\cong SL_2(K)/Z(SL_2(K))=PSL_2(K).}
$$

In characteristic two the scalar center is trivial. The integral formulas avoid the invalid operation of dividing by factorials inside a field of small positive characteristic.

## 4

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [Lie bracket](../../../lie-algebra.md#lie-bracket) is bilinear, so $\operatorname{ad}x$ is a [linear map](../../../vector-space.md#linear-map). Rearranging the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
[x,[y,z]]=[[x,y],z]+[y,[x,z]].
$$

Thus

$$
\boxed{(\operatorname{ad}x)[y,z]=[(\operatorname{ad}x)y,z]+[y,(\operatorname{ad}x)z],}
$$

which is the defining Leibniz rule for a [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra). In particular $\operatorname{ad}x$ is an [inner derivation of a Lie algebra](../../../lie-algebra.md#inner-derivation-of-a-lie-algebra).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Write $D=\operatorname{ad}x$, and choose $N$ with $D^N=0$. The [exponential of a nilpotent Lie algebra derivation](../../../lie-algebra.md#exponential-of-a-nilpotent-lie-algebra-derivation) is the finite [linear operator](../../../vector-space.md#linear-operator)

$$
E=\exp D=\sum_{j=0}^{N-1}\frac{D^j}{j!}.
$$

For a [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra), induction on $k$ using the Leibniz rule and Pascal's identity proves

$$
D^k[y,z]=\sum_{j=0}^k\binom{k}{j}[D^jy,D^{k-j}z].
$$

Expanding $[Ey,Ez]$ and grouping by $k=j+l$ consequently gives

$$
[Ey,Ez]=\sum_{k=0}^{2N-2}\frac1{k!}\sum_{j=0}^k\binom{k}{j}[D^jy,D^{k-j}z]
=\sum_{k=0}^{2N-2}\frac{D^k[y,z]}{k!}=E[y,z].
$$

Terms with an exponent at least $N$ vanish, which justifies extending each inner sum; and $D^k=0$ for $k\ge N$. Finally the finite product of the two exponentials has coefficient

$$
[D^k]\bigl(\exp D\exp(-D)\bigr)=\sum_{j=0}^k\frac{(-1)^{k-j}}{j!(k-j)!}=\frac{(1-1)^k}{k!},
$$

so $\exp(-D)$ is the inverse. We have proved bracket preservation and invertibility, hence **$\exp(\operatorname{ad}x)$ is a Lie algebra automorphism**.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Because $\theta$ is a [Lie algebra automorphism](../../../lie-algebra.md#automorphism-of-a-lie-algebra), for every $y$,

$$
\theta(\operatorname{ad}x)\theta^{-1}y
=\theta[x,\theta^{-1}y]=[\theta x,y]
=(\operatorname{ad}(\theta x))y.
$$

Conjugation therefore also proves that $\operatorname{ad}(\theta x)$ is a [nilpotent operator](../../../linear-operator-theory.md#nilpotent-linear-map), and sends every power of $\operatorname{ad}x$ to the corresponding power of $\operatorname{ad}(\theta x)$. Applying this to the defining finite [exponential of a nilpotent Lie algebra derivation](../../../lie-algebra.md#exponential-of-a-nilpotent-lie-algebra-derivation) yields

$$
\boxed{\theta\exp(\operatorname{ad}x)\theta^{-1}=\exp(\operatorname{ad}(\theta x)).}
$$

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Apply the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) to an arbitrary $z$:

$$
\bigl(\operatorname{ad}x\operatorname{ad}y-\operatorname{ad}y\operatorname{ad}x\bigr)z
=[x,[y,z]]-[y,[x,z]]=[[x,y],z].
$$

Thus the [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) preserves the [Lie bracket](../../../lie-algebra.md#lie-bracket):

$$
\boxed{[\operatorname{ad}x,\operatorname{ad}y]=\operatorname{ad}[x,y].}
$$

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) gives $[L_r,L_s]\subseteq L_{r+s}$ when $r+s\ne0$. The two [roots](../../../semisimple-lie-algebra.md#root-of-a-root-system) are independent, so $r+s\ne0$, and the missing root sum means that this weight space is zero. Hence $[e_r,e_s]=0$. These adjoint root operators are nilpotent: successive brackets shift root weights by the same root, so finite [root strings](../../../semisimple-lie-algebra.md#root-string) force eventual vanishing; on the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) the first bracket lies in its root space and the next is zero. By part (iv), the [nilpotent operators](../../../linear-operator-theory.md#nilpotent-linear-map) $A=t\operatorname{ad}e_r$ and $B=u\operatorname{ad}e_s$ commute. Every power of $A$ therefore commutes with every power of $B$, so their finite [matrix exponentials](../../../linear-operator-theory.md#matrix-exponential) commute too. Using the inverses proved in part (ii),

$$
\boxed{x_s(u)^{-1}x_r(t)^{-1}x_s(u)x_r(t)=I.}
$$

<h3 id="4/vi">vi</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#4/vi)

Let every [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) have squared length $L$. Since $r+s$ is a root, $L=\|r+s\|^2=2L+2(r,s)$, hence $(r,s)=-L/2$. In particular the roots are independent. The potential higher sums satisfy

$$
\|2r+s\|^2=\|r+2s\|^2=3L,
$$

so neither is a root. The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) therefore gives $[e_r,e_{r+s}]=[e_s,e_{r+s}]=0$.

Set $A=t\operatorname{ad}e_r$, $B=u\operatorname{ad}e_s$ and $C=[A,B]=tuN_{r,s}\operatorname{ad}e_{r+s}$. Part (iv) shows $[A,C]=[B,C]=0$. To compute the sign, differentiate $F(v)=e^{-vB}Ae^{vB}$:

$$
F'(v)=e^{-vB}[A,B]e^{vB}=C,\qquad F(0)=A.
$$

Thus $e^{-B}Ae^B=A+C$. Conjugating the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential), and then using the commutation of $A,C$, gives

$$
e^{-B}e^{-A}e^Be^A=e^{-A-C}e^A=e^{-C}.
$$

This proves the [central-commutator exponential identity](../../../lie-algebra.md#central-commutator-exponential-identity) in the required order, and consequently the [simply laced Chevalley commutator formula](../../../semisimple-lie-algebra.md#simply-laced-chevalley-commutator-formula) is

$$
\boxed{x_s(u)^{-1}x_r(t)^{-1}x_s(u)x_r(t)=x_{r+s}(-N_{r,s}tu).}
$$

## 5

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The map $T\mapsto T^{\mathsf T}A+AT$ is linear, so its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) $L$ is a [vector subspace](../../../vector-space.md#vector-subspace) of the [matrix algebra](../../../associative-algebra.md#matrix-algebra). If $T_1,T_2\in L$, use $T_i^{\mathsf T}A=-AT_i$ to compute

$$
\begin{aligned}
[T_1,T_2]^{\mathsf T}A
&=(T_2^{\mathsf T}T_1^{\mathsf T}-T_1^{\mathsf T}T_2^{\mathsf T})A\\
&=-T_2^{\mathsf T}AT_1+T_1^{\mathsf T}AT_2\\
&=AT_2T_1-AT_1T_2=-A[T_1,T_2].
\end{aligned}
$$

Thus $L$ is closed under the [commutator](../../../lie-algebra.md#commutator). This bracket is bilinear and satisfies $[T,T]=0$. Associativity of matrix multiplication gives the [Jacobi identity](../../../lie-algebra.md#jacobi-identity): expanding $[T_1,[T_2,T_3]]+[T_2,[T_3,T_1]]+[T_3,[T_1,T_2]]$ makes each of the six ordered triple products occur once with each sign. Therefore **$L$ is a Lie algebra**. No nonsingularity or symmetry assumption on $A$ was needed.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

For the [nilpotent matrix](../../../linear-operator-theory.md#nilpotent-matrix) $T$, define the polynomial $E(z)=\sum_{k=0}^{m-1}z^kT^k/k!$. Because $T^m=0$, differentiating gives $E'(z)=TE(z)=E(z)T$. The derivative of the preserved [bilinear form](../../../linear-algebra.md#bilinear-form) matrix is therefore

$$
\frac{d}{dz}\bigl(E(z)^{\mathsf T}AE(z)\bigr)
=E(z)^{\mathsf T}(T^{\mathsf T}A+AT)E(z)=0.
$$

It is a constant matrix polynomial, equal to $A$ at $z=0$. Evaluation at one proves

$$
\boxed{(\exp T)^{\mathsf T}A\exp T=A.}
$$

Also $E(-1)$ is the inverse of $E(1)$ by the finite exponential product identity, so this really is an invertible isometry, even when $A$ is degenerate.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Write $T=\begin{pmatrix}P&Q\\R&S\end{pmatrix}$ and $J=\begin{pmatrix}0&I_l\\-I_l&0\end{pmatrix}$. Block multiplication gives

$$
T^{\mathsf T}J+JT=
\begin{pmatrix}R-R^{\mathsf T}&P^{\mathsf T}+S\\-S^{\mathsf T}-P&Q^{\mathsf T}-Q\end{pmatrix}.
$$

Its vanishing is equivalent to

$$
\boxed{S=-P^{\mathsf T},\qquad Q=Q^{\mathsf T},\qquad R=R^{\mathsf T}.}
$$

This identifies $L$ with the [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra) $\mathfrak{sp}_{2l}(\mathbb C)$.

We now supply the requested [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition), including explicit vectors. Let $E_{ab}$ be the [matrix units](../../../vector-space.md#matrix-unit), put $h_i=E_{ii}-E_{l+i,l+i}$, and define the [linear functionals](../../../linear-algebra.md#linear-functional) $\varepsilon_i$ on the diagonal [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) by $\varepsilon_i(h)=\lambda_i$. Then $H=\bigoplus_i\mathbb C h_i$. The [Cn root system](../../../semisimple-lie-algebra.md#cn-root-system) and a corresponding [matrix root basis of the symplectic Lie algebra](../../../semisimple-lie-algebra.md#matrix-root-basis-of-the-symplectic-lie-algebra) are

$$
\begin{aligned}
e_{\varepsilon_i-\varepsilon_j}&=E_{ij}-E_{l+j,l+i} &&(i\ne j),\\
e_{\varepsilon_i+\varepsilon_j}&=E_{i,l+j}+E_{j,l+i} &&(i<j),\\
e_{-\varepsilon_i-\varepsilon_j}&=E_{l+i,j}+E_{l+j,i} &&(i<j),\\
e_{2\varepsilon_i}&=E_{i,l+i},\qquad e_{-2\varepsilon_i}=E_{l+i,i}.&&
\end{aligned}
$$

Each listed vector satisfies the block conditions just proved. For a diagonal matrix $h$, the [matrix unit](../../../vector-space.md#matrix-unit) calculation $[h,E_{ab}]=(h_{aa}-h_{bb})E_{ab}$ gives all the requested [eigenvalues](../../../linear-operator-theory.md#eigenvalue) explicitly:

$$
\begin{aligned}
[h,e_{\varepsilon_i-\varepsilon_j}]&=(\lambda_i-\lambda_j)e_{\varepsilon_i-\varepsilon_j},\\
[h,e_{\varepsilon_i+\varepsilon_j}]&=(\lambda_i+\lambda_j)e_{\varepsilon_i+\varepsilon_j},\\
[h,e_{-\varepsilon_i-\varepsilon_j}]&=-(\lambda_i+\lambda_j)e_{-\varepsilon_i-\varepsilon_j},\\
[h,e_{2\varepsilon_i}]&=2\lambda_i e_{2\varepsilon_i},\qquad
[h,e_{-2\varepsilon_i}]=-2\lambda_i e_{-2\varepsilon_i}.
\end{aligned}
$$

The diagonal vectors and difference-root vectors span every possible $P$ block. The sum-root and doubled-root vectors span all symmetric $Q$ and $R$ blocks. They are [linearly independent](../../../vector-space.md#linear-independence), as is evident from their disjoint independent block entries. Equivalently there are $l+2l^2=l(2l+1)$ of them, exactly the [dimension](../../../vector-space.md#dimension-vector-space) $l^2+2l(l+1)/2$ of $L$. The zero weight space is precisely $H$: a zero weight forces $P$ diagonal and every entry of $Q,R$ to vanish. Hence every nonzero [root space](../../../semisimple-lie-algebra.md#root-space) is one-dimensional and

$$
\boxed{L=H\oplus\bigoplus_{r\in\{\pm(\varepsilon_i\pm\varepsilon_j):i<j\}\cup\{\pm2\varepsilon_i\}}\mathbb C e_r,\qquad [h,e_r]=r(h)e_r.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
