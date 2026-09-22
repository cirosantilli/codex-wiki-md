# Paper 28

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_28.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_28.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A set $S$ of [prime numbers](../../../number-theory.md#prime-number) has [Dirichlet density](../../../algebraic-number-theory.md#dirichlet-density) $\delta$ if the following limit exists:

$$
\delta(S)=\lim_{s\downarrow1}\frac{\sum_{p\in S}p^{-s}}{\log(1/(s-1))}=\delta.
$$

Equivalently, the denominator can be $\sum_p p^{-s}$, since that sum is $\log(1/(s-1))+O(1)$. Adding or removing finitely many [prime numbers](../../../number-theory.md#prime-number) leaves the [Dirichlet density](../../../algebraic-number-theory.md#dirichlet-density) unchanged.

Put $\alpha=\sqrt[4]{2}>0$ and $L=\mathbb Q(\alpha,i)$. This is the [splitting field](../../../galois-theory.md#splitting-field) of $X^4-2$, whose four [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial) are $\alpha,i\alpha,-\alpha,-i\alpha$. The polynomial is an [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial) at $2$, so $[\mathbb Q(\alpha):\mathbb Q]=4$. Since $\mathbb Q(\alpha)$ is contained in the [real numbers](../../../arithmetic.md#real-number), it does not contain $i$, giving $[L:\mathbb Q]=8$. Thus $L/\mathbb Q$ is a [Galois extension](../../../galois-theory.md#finite-galois-extension) of degree $8$. Its [Galois group](../../../galois-theory.md#galois-group) is the [dihedral group](../../../finite-group-theory.md#dihedral-group) of order $8$: the [field automorphisms](../../../galois-theory.md#field-automorphism) $r(\alpha)=i\alpha$, $r(i)=i$ and $s(\alpha)=\alpha$, $s(i)=-i$ satisfy $r^4=s^2=1$ and $srs=r^{-1}$.

For an odd [prime number](../../../number-theory.md#prime-number) $p$, the condition $p\equiv1\pmod4$ means that the [finite field](../../../algebra.md#finite-field) $\mathbb F_p$ contains all fourth [roots of unity](../../../algebra.md#root-of-unity). Under this condition, $2$ is a [quartic residue](../../../algebra.md#quartic-residue) exactly when $X^4-2$ has a root in $\mathbb F_p$; multiplying that root by $1,i,-1,-i$ gives all four distinct roots. Conversely, complete splitting of $X^4-2$ over $\mathbb F_p$ gives both a fourth root of $2$ and a primitive fourth [root of unity](../../../algebra.md#root-of-unity), so it also forces $p\equiv1\pmod4$.

The [polynomial discriminant](../../../galois-theory.md#polynomial-discriminant) of $X^4-2$ is $-2^{11}$. Hence every odd [prime number](../../../number-theory.md#prime-number) is unramified in $L$, and the root-splitting criterion is equivalent to its [Frobenius automorphism](../../../arithmetic.md#frobenius-automorphism) acting trivially on all the roots. Since the roots generate $L$, this is equivalent to the [Frobenius automorphism](../../../arithmetic.md#frobenius-automorphism) being the identity, or to $p$ being a [completely split prime](../../../algebraic-number-theory.md#completely-split-prime) of $L/\mathbb Q$. The [Chebotarev density theorem](../../../algebraic-number-theory.md#chebotarev-density-theorem) says that the unramified [prime numbers](../../../number-theory.md#prime-number) with [Frobenius conjugacy class](../../../arithmetic.md#frobenius-conjugacy-class) $C$ have [Dirichlet density](../../../algebraic-number-theory.md#dirichlet-density) $|C|/|\operatorname{Gal}(L/\mathbb Q)|$. Here $C=\{1\}$, so

$$
\boxed{\delta(S)=\frac18.}
$$

## 2

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A normalization is important here. I use the [covolume-one theta function of a fractional ideal](../../../modular-function.md#covolume-one-theta-function-of-a-fractional-ideal), for which the requested limit is $1$, and also give the formula for the unnormalized [Gaussian theta sum](../../../modular-function.md#gaussian-theta-sum).

Let $n=[K:\mathbb Q]$, let $d_v=[K_v:\mathbb R]\in\{1,2\}$, and choose one [field embedding](../../../galois-theory.md#field-embedding) $\sigma_v$ for each [Archimedean place](../../../algebraic-number-theory.md#archimedean-place). The [Minkowski embedding of a number field](../../../algebraic-number-theory.md#minkowski-embedding-of-a-number-field) identifies

$$
K_\infty=\mathbb R^{r_1}\times\mathbb C^{r_2},\qquad n=r_1+2r_2,
$$

with a real [inner product space](../../../linear-algebra.md#inner-product-space) having

$$
\langle x,z\rangle=\sum_{v\text{ real}}x_vz_v+2\sum_{v\text{ complex}}\operatorname{Re}(x_v\overline{z_v}),\qquad |x|^2=\sum_vd_v|x_v|^2.
$$

Its Euclidean [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) is $d\mu=\prod_{v\text{ real}}dx_v\prod_{v\text{ complex}}2\,d\operatorname{Re}x_v\,d\operatorname{Im}x_v$. With this convention, the [covolume of a fractional ideal lattice](../../../algebraic-number-theory.md#covolume-of-a-fractional-ideal-lattice) $j(\mathfrak b)$ is

$$
C_{\mathfrak b}=\sqrt{|D_K|}\,N(\mathfrak b),
$$

where $D_K$ is the [field discriminant](../../../algebraic-number-theory.md#field-discriminant) and $N(\mathfrak b)$ is the positive absolute [norm of a fractional ideal](../../../algebraic-number-theory.md#norm-of-a-fractional-ideal). Thus the [Euclidean lattice](../../../fourier-analysis.md#euclidean-lattice) $\Lambda_{\mathfrak b}=C_{\mathfrak b}^{-1/n}j(\mathfrak b)$ has [covolume](../../../fourier-analysis.md#covolume) $1$. Define

$$
\boxed{\Theta(y,\mathfrak b)=\sum_{a\in\mathfrak b}\exp\left(-\pi C_{\mathfrak b}^{-2/n}\sum_{v\in S_\infty}d_vy_v|\sigma_v(a)|^2\right).}
$$

This [Gaussian theta sum](../../../modular-function.md#gaussian-theta-sum) converges absolutely whenever every $y_v>0$.

The [trace dual of a fractional ideal](../../../algebraic-number-theory.md#trace-dual-of-a-fractional-ideal) is

$$
\mathfrak b^\vee=\mathfrak D_{K/\mathbb Q}^{-1}\mathfrak b^{-1}=\{z\in K:\operatorname{Tr}_{K/\mathbb Q}(z\mathfrak b)\subseteq\mathbb Z\}.
$$

Here $\mathfrak D_{K/\mathbb Q}^{-1}$ is the [inverse different](../../../arithmetic.md#inverse-different). Since $N(\mathfrak D_{K/\mathbb Q})=|D_K|$, we have $C_{\mathfrak b^\vee}=C_{\mathfrak b}^{-1}$. There is a subtle distinction between the [trace pairing](../../../algebraic-number-theory.md#trace-pairing) and the positive [inner product](../../../linear-algebra.md#inner-product): the [dual lattice](../../../fourier-analysis.md#dual-lattice) of $j(\mathfrak b)$ is $\overline{j(\mathfrak b^\vee)}$, where the bar conjugates the complex coordinates and fixes the real ones. Indeed,

$$
\langle j(a),\overline{j(z)}\rangle=\operatorname{Tr}_{K/\mathbb Q}(az).
$$

Consequently $\Lambda_{\mathfrak b}^*=\overline{\Lambda_{\mathfrak b^\vee}}$. Coordinatewise [complex conjugation](../../../complex-analysis.md#complex-conjugation) preserves the weighted squared lengths in the [Gaussian theta sum](../../../modular-function.md#gaussian-theta-sum).

Here are the precise analytic formulas used in the proof. For a [Schwartz function](../../../fourier-analysis.md#schwartz-function) on $K_\infty$, take the [Fourier transform](../../../analysis.md#fourier-transform) to be

$$
\widehat f(z)=\int_{K_\infty}f(x)e^{-2\pi i\langle x,z\rangle}\,d\mu(x).
$$

For a full [Euclidean lattice](../../../fourier-analysis.md#euclidean-lattice) $\Lambda$ of [covolume](../../../fourier-analysis.md#covolume) $C$, the [Poisson summation formula for a Euclidean lattice](../../../fourier-analysis.md#poisson-summation-formula-for-a-euclidean-lattice) is

$$
\sum_{x\in\Lambda}f(x)=C^{-1}\sum_{z\in\Lambda^*}\widehat f(z).
$$

For $f_y(x)=\exp(-\pi\sum_vd_vy_v|x_v|^2)$, the [Gaussian Fourier transform](../../../fourier-analysis.md#fourier-transform-of-a-gaussian), applied in orthonormal real coordinates, gives

$$
\widehat f_y(z)=\|y\|^{-1/2}\exp\left(-\pi\sum_vd_vy_v^{-1}|z_v|^2\right),\qquad \|y\|=\prod_vy_v^{d_v}.
$$

More generally, $\widehat{\exp(-\pi x^TAx)}(z)=(\det A)^{-1/2}\exp(-\pi z^TA^{-1}z)$ for a real [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) $A$ that is symmetric. Each complex coordinate contributes two real coordinates, which explains its exponent $d_v=2$.

Apply the [Poisson summation formula for a Euclidean lattice](../../../fourier-analysis.md#poisson-summation-formula-for-a-euclidean-lattice) to $\Lambda_{\mathfrak b}$, whose [covolume](../../../fourier-analysis.md#covolume) is $1$, and use the preceding description of its [dual lattice](../../../fourier-analysis.md#dual-lattice). The [anisotropic theta functional equation](../../../modular-function.md#anisotropic-theta-functional-equation) is

$$
\boxed{\Theta(y,\mathfrak b)=\|y\|^{-1/2}\Theta(y^{-1},\mathfrak b^\vee),\qquad (y^{-1})_v=y_v^{-1}.}
$$

For comparison, the unnormalized [Gaussian theta sum](../../../modular-function.md#gaussian-theta-sum)

$$
\theta(y,\mathfrak b)=\sum_{a\in\mathfrak b}\exp\left(-\pi\sum_vd_vy_v|\sigma_v(a)|^2\right)
$$

has the [functional equation](../../../analysis.md#functional-equation)

$$
\theta(y,\mathfrak b)=C_{\mathfrak b}^{-1}\|y\|^{-1/2}\theta(y^{-1},\mathfrak b^\vee),
$$

and its corresponding limit is $C_{\mathfrak b}^{-1}$ rather than $1$. Explicitly, our normalization is $\Theta(y,\mathfrak b)=\theta(C_{\mathfrak b}^{-2/n}y,\mathfrak b)$.

For the [small-parameter asymptotic of a lattice theta sum](../../../modular-function.md#small-parameter-asymptotic-of-a-lattice-theta-sum), $y\to0$ means that every coordinate tends to zero. In $\Theta(y^{-1},\mathfrak b^\vee)$, the zero lattice vector contributes $1$. Every nonzero vector contributes a term tending to zero. Once every $y_v\leq1$, all these terms are bounded by the summable [Gaussian theta sum](../../../modular-function.md#gaussian-theta-sum) $\sum_{\lambda\in\Lambda_{\mathfrak b^\vee}}e^{-\pi|\lambda|^2}$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) therefore gives $\Theta(y^{-1},\mathfrak b^\vee)\to1$. Using the [anisotropic theta functional equation](../../../modular-function.md#anisotropic-theta-functional-equation),

$$
\boxed{\lim_{y\to0}\|y\|^{1/2}\Theta(y,\mathfrak b)=1.}
$$

The condition that every coordinate tends to zero matters; $\|y\|\to0$ alone would not justify this argument.

## 3

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a finite extension $E/K$ of [number fields](../../../algebraic-number-theory.md#number-field), the [inverse different](../../../arithmetic.md#inverse-different) is the [fractional ideal](../../../commutative-algebra.md#fractional-ideal)

$$
\mathfrak D_{E/K}^{-1}=\{x\in E:\operatorname{Tr}_{E/K}(x\mathcal O_E)\subseteq\mathcal O_K\}.
$$

The [different ideal](../../../arithmetic.md#different-ideal) is its inverse. The [trace pairing](../../../algebraic-number-theory.md#trace-pairing) is nondegenerate because extensions of [number fields](../../../algebraic-number-theory.md#number-field) are separable, so this definition gives a full [fractional ideal](../../../commutative-algebra.md#fractional-ideal). The inclusion $\mathcal O_E\subseteq\mathfrak D_{E/K}^{-1}$ shows that $\mathfrak D_{E/K}$ is integral.

Write its [prime ideal factorization](../../../algebraic-number-theory.md#prime-ideal-factorization) as $\mathfrak D_{E/K}=\prod_{\mathfrak P}\mathfrak P^{d_{\mathfrak P}}$. For $\mathfrak P$ above $\mathfrak p$, with [ramification index](../../../arithmetic.md#ramification-index) $e_{\mathfrak P}$ and residue characteristic $\ell$, the [different exponent and tame ramification](../../../arithmetic.md#different-exponent-and-tame-ramification) theorem says

$$
\boxed{d_{\mathfrak P}\geq e_{\mathfrak P}-1,\qquad d_{\mathfrak P}=e_{\mathfrak P}-1\ \Longleftrightarrow\ \ell\nmid e_{\mathfrak P}.}
$$

The equivalence uses the separability of finite residue-field extensions. In particular, $d_{\mathfrak P}=0$ precisely at unramified [prime ideals](../../../commutative-algebra.md#prime-ideal); in the wild case $d_{\mathfrak P}\geq e_{\mathfrak P}$. This theorem does not require a [Galois extension](../../../galois-theory.md#finite-galois-extension). The [relative discriminant](../../../algebraic-number-theory.md#relative-discriminant) is the [norm of the different ideal](../../../algebraic-number-theory.md#norm-of-the-different-ideal):

$$
\mathfrak d_{E/K}=N_{E/K}(\mathfrak D_{E/K}).
$$

For $K=\mathbb Q$, this gives $|D_E|=N(\mathfrak D_{E/\mathbb Q})$.

Now take $\alpha^3=m$ and $K=\mathbb Q(\alpha)$. For any [prime number](../../../number-theory.md#prime-number) $q\mid m$, the [square-free integer](../../../number-theory.md#square-free-integer) hypothesis makes $X^3-m$ an [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial) at $q$. It is therefore irreducible, and $K$ is a [pure cubic number field](../../../algebraic-number-theory.md#pure-cubic-number-field) of degree $3$. Since $\alpha$ is an [algebraic integer](../../../algebraic-number-theory.md#algebraic-integer), $A=\mathbb Z[\alpha]$ is an [order in a number field](../../../algebraic-number-theory.md#order-in-a-number-field). The [discriminant of elements of a number field](../../../algebraic-number-theory.md#discriminant-of-elements-of-a-number-field) for its basis $1,\alpha,\alpha^2$ is

$$
\operatorname{disc}(1,\alpha,\alpha^2)=\operatorname{disc}(X^3-m)=-27m^2.
$$

For example, the resultant of $X^3-m$ and $3X^2$ is $27m^2$, and the degree-three sign in the [polynomial discriminant](../../../galois-theory.md#polynomial-discriminant) is negative. If $I=[\mathcal O_K:A]$, the [discriminant-index formula for an integral lattice](../../../algebraic-number-theory.md#discriminant-index-formula-for-an-integral-lattice) gives

$$
-27m^2=I^2D_K.
$$

Only [prime numbers](../../../number-theory.md#prime-number) dividing $3m$ can therefore divide $I$.

For $q\mid m$, the [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial) gives a [totally ramified extension](../../../arithmetic.md#totally-ramified-extension) of $\mathbb Q_q$ of degree $3$. Thus $K$ has a unique [prime ideal](../../../commutative-algebra.md#prime-ideal) $\mathfrak P$ above $q$, with [ramification index](../../../arithmetic.md#ramification-index) $3$ and [residue-field degree](../../../arithmetic.md#residue-field-degree) $1$. Since $q\ne3$, this is [tame ramification](../../../arithmetic.md#tamely-ramified-extension), and the [different exponent and tame ramification](../../../arithmetic.md#different-exponent-and-tame-ramification) theorem gives $d_{\mathfrak P}=2$. Hence $v_q(D_K)=2$. Comparing with $v_q(-27m^2)=2$ in the [discriminant-index formula for an integral lattice](../../../algebraic-number-theory.md#discriminant-index-formula-for-an-integral-lattice) yields $v_q(I)=0$.

At $3$, use the [shifted Eisenstein polynomial](../../../arithmetic.md#shifted-eisenstein-polynomial) of $\beta=\alpha-m$:

$$
(T+m)^3-m=T^3+3mT^2+3m^2T+(m^3-m).
$$

Because $3\nmid m$, the constant term is divisible by $3$. Moreover,

$$
9\mid m^3-m\ \Longleftrightarrow\ m\equiv\pm1\pmod9
$$

when $3\nmid m$: the factors $m-1$ and $m+1$ cannot both be divisible by $3$. The hypotheses therefore give $v_3(m^3-m)=1$, so the translated polynomial is an [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial) at $3$. The resulting completion is a [totally ramified extension](../../../arithmetic.md#totally-ramified-extension) of degree $3$, with [residue-field degree](../../../arithmetic.md#residue-field-degree) $1$, and its [ramification index](../../../arithmetic.md#ramification-index) is divisible by the residue characteristic. Thus its [different exponent](../../../arithmetic.md#different-exponent) is at least $3$.

It follows that $v_3(D_K)\geq3$. But $v_3(-27m^2)=3$, so

$$
3=2v_3(I)+v_3(D_K)
$$

forces $v_3(I)=0$ and $v_3(D_K)=3$. No [prime number](../../../number-theory.md#prime-number) divides $I$. We have proved the [integral basis of a nonexceptional pure cubic field](../../../algebraic-number-theory.md#integral-basis-of-a-nonexceptional-pure-cubic-field):

$$
\boxed{\mathcal O_K=\mathbb Z[\alpha],\qquad \{1,\alpha,\alpha^2\}\text{ is an integral basis},\qquad D_K=-27m^2.}
$$

Using local [Eisenstein polynomials](../../../arithmetic.md#eisenstein-polynomial) here only establishes the local [ramification indices](../../../arithmetic.md#ramification-index); it does not assume that $\mathbb Z[\alpha]$ is already the full [ring of integers of a number field](../../../algebraic-number-theory.md#ring-of-integers).

## 4

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Here a divisor is a [modulus of a number field](../../../algebraic-number-theory.md#modulus-of-a-number-field), rather than an arbitrary real-weighted divisor. Write

$$
\mathfrak c=\mathfrak c_0\mathfrak c_\infty,\qquad \mathfrak c_0=\prod_{\mathfrak p}\mathfrak p^{m_{\mathfrak p}},
$$

where $\mathfrak c_0$ is a nonzero [integral ideal](../../../commutative-algebra.md#integral-ideal), the finite multiplicities $m_{\mathfrak p}$ are nonnegative integers, and $\mathfrak c_\infty$ is a set of real [Archimedean places](../../../algebraic-number-theory.md#archimedean-place). The [multiplicity of a place in a modulus](../../../algebraic-number-theory.md#multiplicity-of-a-place-in-a-modulus) is $m_v(\mathfrak c)=m_{\mathfrak p}$ at the finite place corresponding to $\mathfrak p$, is $1$ at a real place in $\mathfrak c_\infty$, and is $0$ at every other infinite place. In particular complex places have multiplicity $0$.

Let $I_{\mathfrak c}$ be the group of nonzero [fractional ideals](../../../commutative-algebra.md#fractional-ideal) prime to $\mathfrak c_0$. Put

$$
K_{\mathfrak c,1}^{\times}=\{a\in K^{\times}:v_{\mathfrak p}(a-1)\geq m_{\mathfrak p}\text{ for }\mathfrak p\mid\mathfrak c_0,\quad \sigma_v(a)>0\text{ for }v\in\mathfrak c_\infty\}.
$$

Let $P_{\mathfrak c}$ consist of the [principal ideals](../../../commutative-algebra.md#principal-ideal) $(a)$ with $a\in K_{\mathfrak c,1}^{\times}$. The [generalized ideal class group](../../../algebraic-number-theory.md#ray-class-group) is the [ray class group](../../../algebraic-number-theory.md#ray-class-group)

$$
\boxed{H_{\mathfrak c}=I_{\mathfrak c}/P_{\mathfrak c}.}
$$

Let $U=\mathcal O_K^{\times}$ be the [unit group](../../../algebra.md#unit-group), let $U_{\mathfrak c}=U\cap K_{\mathfrak c,1}^{\times}$ be the group of [ray units](../../../algebraic-number-theory.md#ray-unit), and define the [residue and signature group of a modulus](../../../algebraic-number-theory.md#residue-and-signature-group-of-a-modulus)

$$
G_{\mathfrak c}=(\mathcal O_K/\mathfrak c_0)^{\times}\times\{\pm1\}^{\mathfrak c_\infty}.
$$

The first factor is omitted when $\mathfrak c_0=\mathcal O_K$. There is a [group homomorphism](../../../group-theory.md#group-homomorphism) $\rho:U\to G_{\mathfrak c}$ recording the unit's finite residues and its signs. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is $U_{\mathfrak c}$.

Let $P^{\mathfrak c}$ consist of all [principal fractional ideals](../../../commutative-algebra.md#principal-fractional-ideal) prime to $\mathfrak c_0$, and put $R_{\mathfrak c}=P^{\mathfrak c}/P_{\mathfrak c}$. The two [short exact sequences](../../../module-theory.md#short-exact-sequence) are

$$
\boxed{1\longrightarrow U/U_{\mathfrak c}\xrightarrow{\rho}G_{\mathfrak c}\longrightarrow R_{\mathfrak c}\longrightarrow1,}
$$

and

$$
\boxed{1\longrightarrow R_{\mathfrak c}\longrightarrow H_{\mathfrak c}\longrightarrow\operatorname{Cl}(\mathcal O_K)\longrightarrow1.}
$$

For the first [short exact sequence](../../../module-theory.md#short-exact-sequence), [weak approximation for number fields](../../../algebraic-number-theory.md#weak-approximation-for-number-fields) realizes every choice of finite unit residues and real signs by some $a\in K^{\times}$ prime to $\mathfrak c_0$. Send that data to the class of $(a)$ in $R_{\mathfrak c}$. Changing $a$ without changing its residues and signs multiplies it by an element of $K_{\mathfrak c,1}^{\times}$, so the map is well-defined. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) consists exactly of data arising from units: if $(a)=(b)$ with $b\in K_{\mathfrak c,1}^{\times}$, then $a/b\in U$. This gives $R_{\mathfrak c}\cong G_{\mathfrak c}/\rho(U)$. For the second [short exact sequence](../../../module-theory.md#short-exact-sequence), forget the ray conditions. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is $R_{\mathfrak c}$, and [weak approximation for number fields](../../../algebraic-number-theory.md#weak-approximation-for-number-fields) gives a representative prime to $\mathfrak c_0$ for every [ideal class](../../../algebraic-number-theory.md#ideal-class). These are the two parts of the [ray class exact sequence](../../../algebraic-number-theory.md#ray-class-exact-sequence).

For $K=\mathbb Q(\sqrt{15})$, the [ring of integers of a quadratic field](../../../algebraic-number-theory.md#ring-of-integers-of-a-quadratic-field) is $\mathcal O_K=\mathbb Z[\sqrt{15}]$. The finite modulus is trivial and both real places occur, so $H_{\mathfrak c}$ is the [narrow ideal class group](../../../algebraic-number-theory.md#narrow-ideal-class-group) and $G_{\mathfrak c}=\{\pm1\}^2$. The two [field embeddings](../../../galois-theory.md#field-embedding) send $\sqrt{15}$ to $\sqrt{15}$ and $-\sqrt{15}$. The given unit $\epsilon=4+\sqrt{15}$ is positive at both places, since $4-\sqrt{15}>0$; the unit $-1$ is negative at both. Thus the [unit signature map](../../../algebra.md#unit-signature-map) has image

$$
\rho(U)=\{(+,+),(-,-)\},\qquad |R_{\mathfrak c}|=\frac42=2.
$$

The given [ideal class group](../../../algebraic-number-theory.md#ideal-class-group) has order $2$. The second [short exact sequence](../../../module-theory.md#short-exact-sequence) therefore gives

$$
\boxed{|H_{\mathfrak c}|=2\cdot2=4.}
$$

To determine the group structure, retain the ideal $\mathfrak p=(2,1+\sqrt{15})$ that generates the ordinary [ideal class group](../../../algebraic-number-theory.md#ideal-class-group). We have $\mathfrak p^2=(2)$: all generators $4$, $2(1+\sqrt{15})$ and $(1+\sqrt{15})^2$ lie in $(2)$, while

$$
(1+\sqrt{15})^2-2(1+\sqrt{15})-3\cdot4=2
$$

puts $2$ in $\mathfrak p^2$. Since $2$ is [totally positive](../../../algebraic-number-theory.md#totally-positive-element-of-a-number-field), $[\mathfrak p]^2=1$ in the [narrow ideal class group](../../../algebraic-number-theory.md#narrow-ideal-class-group). Its image in the ordinary [ideal class group](../../../algebraic-number-theory.md#ideal-class-group) is nontrivial, so $[\mathfrak p]$ has order exactly $2$.

The class of the [principal ideal](../../../commutative-algebra.md#principal-ideal) $(\sqrt{15})$ is a nontrivial element of $R_{\mathfrak c}$. Its two signs are $(+,-)$, and multiplying by a unit can only reverse both signs or neither, so no generator of this ideal is [totally positive](../../../algebraic-number-theory.md#totally-positive-element-of-a-number-field). Its square is $(15)$, which does have a [totally positive](../../../algebraic-number-theory.md#totally-positive-element-of-a-number-field) generator. Thus $[(\sqrt{15})]$ is another element of order $2$, distinct from $[\mathfrak p]$ because its ordinary [ideal class](../../../algebraic-number-theory.md#ideal-class) is trivial. These two elements are independent and generate all four classes. Consequently

$$
\boxed{H_{\mathfrak c}\cong(\mathbb Z/2\mathbb Z)^2.}
$$

The nontrivial ordinary [ideal class](../../../algebraic-number-theory.md#ideal-class) already has a lift of order $2$, so the extension in the second [short exact sequence](../../../module-theory.md#short-exact-sequence) splits; it cannot be cyclic of order $4$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
