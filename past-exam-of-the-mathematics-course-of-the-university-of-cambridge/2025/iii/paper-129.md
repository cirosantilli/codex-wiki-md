# Paper 129

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20129.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20129.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 129](paper-129.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Freiman-Ruzsa theorem over a finite field](../../../additive-combinatorics.md#freiman-ruzsa-theorem-over-a-finite-field) states that if $A\subseteq\mathbb F_p^n$ and $|A+A|\leq K|A|$, then $A$ is contained in a [vector subspace](../../../vector-space.md#vector-subspace) $H$ with

$$
|H|\leq K^2p^{K^4}|A|.
$$

After translating $A$, assume $0\in A$. Put $S=A-A$, and choose $X\subseteq A+S$ maximal subject to the translates $x+A$, $x\in X$, being pairwise disjoint. Since $X+A\subseteq2A+S=3A-A$, the [Plünnecke-Ruzsa inequality](../../../additive-combinatorics.md#plunnecke-ruzsa-inequality) gives

$$
|X||A|=|X+A|\leq|3A-A|\leq K^4|A|,
$$

so $|X|\leq K^4$.

Maximality gives $A+S\subseteq X+S$: if $y\in A+S$ is not already in $X$, then $(y+A)\cap(x+A)\ne\varnothing$ for some $x\in X$, whence $y\in x+A-A=x+S$. Inductively, $mA+S\subseteq\langle X\rangle+S$ for every positive integer $m$. Because $0\in A$, every element of $\langle A\rangle$ belongs to some $mA$ in the finite vector space, and therefore

$$
H:=\langle A\rangle\subseteq\langle X\rangle+S.
$$

Finally, $|\langle X\rangle|\leq p^{|X|}$ and $|S|\leq K^2|A|$ by the Plünnecke-Ruzsa inequality, so

$$
\boxed{|H|\leq p^{|X|}|S|\leq K^2p^{K^4}|A|.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $H\leq\mathbb F_p^n$ be a subspace with $|H|$ much larger than $K^2$, and choose linearly independent vectors $e_1,\ldots,e_{K-1}$ whose images are independent modulo $H$. Set

$$
A=H\cup\{e_1,\ldots,e_{K-1}\}.
$$

Then $|A|=|H|+K-1\sim|H|$, while $A+A$ is the union of $H$, the $K-1$ disjoint cosets $e_i+H$, and at most $K^2$ exceptional sums $e_i+e_j$. Hence

$$
|A+A|\sim K|A|.
$$

Every subspace containing $A$ must contain $H$ and all $e_i$, so it has at least $p^{K-1}|H|\sim p^{K-1}|A|$ elements. Thus the exponential dependence on $K$ in the [Freiman-Ruzsa theorem over a finite field](../../../additive-combinatorics.md#freiman-ruzsa-theorem-over-a-finite-field) cannot in general be replaced by a subexponential one.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The hypothesis says that the normalized [additive energy](../../../additive-combinatorics.md#additive-energy) of $A$ is at least $\eta$. By the [Balog-Szemerédi-Gowers theorem](../../../additive-combinatorics.md#balog-szemeredi-gowers-theorem), for an absolute $C_0$ there is $A'\subseteq A$ such that

$$
|A'|\geq\eta^{C_0}|A|,
\qquad
|A'+A'|\leq\eta^{-C_0}|A'|.
$$

The finite-field Bogolyubov-Ruzsa consequence of the [Freiman-Ruzsa theorem over a finite field](../../../additive-combinatorics.md#freiman-ruzsa-theorem-over-a-finite-field) says that a set of doubling at most $K$ has a [vector subspace](../../../vector-space.md#vector-subspace)

$$
V\subseteq A'+A'-A'-A'
$$

with $|V|\geq p^{-K^{C_1}}|A'|$ for an absolute $C_1$. Taking $K=\eta^{-C_0}$ and enlarging the absolute exponent gives

$$
V\subseteq A+A-A-A,
\qquad
|V|\geq p^{-\eta^{-C}}|A|.
$$

This is an energy form of the [Bogolyubov lemma](../../../additive-combinatorics.md#bogolyubov-lemma): the usual lemma assumes positive density in an ambient group, whereas the [Balog-Szemerédi-Gowers theorem](../../../additive-combinatorics.md#balog-szemeredi-gowers-theorem) first extracts a dense structured model from the many additive quadruples. The resulting bound depends on the energy parameter rather than on the possibly tiny ambient density of $A$.

## 2

↑ **Parent:** [Paper 129](paper-129.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For $\Gamma\subseteq\widehat G$ and $\rho>0$, the [Bohr set](../../../additive-combinatorics.md#bohr-set) is

$$
B(\Gamma,\rho)
=\{x\in G:|\gamma(x)-1|\leq\rho\text{ for every }\gamma\in\Gamma\}.
$$

Writing $d=|\Gamma|$, the [lower bound for the size of a Bohr set](../../../additive-combinatorics.md#lower-bound-for-the-size-of-a-bohr-set) is

$$
\boxed{|B(\Gamma,\rho)|\geq
\left(\frac{\rho}{8}\right)^d|G|.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use normalized convolution and [Fourier coefficients](../../../analysis.md#fourier-transform), and define the large spectrum

$$
\Gamma=\{\gamma\in\widehat G:|\widehat f(\gamma)|\geq\epsilon\delta\}.
$$

By the [Parseval identity](../../../fourier-analysis.md#parseval-identity) and $0\leq f\leq1$,

$$
|\Gamma|\epsilon^2\delta^2
\leq\sum_\gamma|\widehat f(\gamma)|^2
=\mathbb E f^2
\leq\delta,
$$

so $|\Gamma|\leq\epsilon^{-2}\delta^{-1}$.

The [convolution theorem](../../../fourier-analysis.md#convolution-theorem) gives

$$
(f*f*f)(x+y)-(f*f*f)(x)
=\sum_\gamma\widehat f(\gamma)^3\gamma(x)(\gamma(y)-1).
$$

If $y\in B(\Gamma,\epsilon)$, the part over $\Gamma$ is at most

$$
\epsilon\sum_{\gamma\in\Gamma}|\widehat f(\gamma)|^3
\leq\epsilon\delta\sum_\gamma|\widehat f(\gamma)|^2
\leq\epsilon\delta^2,
$$

because $|\widehat f(\gamma)|\leq\delta$. On the complementary spectrum, $|\widehat f(\gamma)|<\epsilon\delta$ and $|\gamma(y)-1|\leq2$, so the contribution is less than $2\epsilon\delta^2$. The required difference is therefore less than $3\epsilon\delta^2$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Apply the preceding Fourier argument to $f=1_A$, retaining the frequencies needed to make the oscillation of $1_A*1_A*1_A$ strictly smaller than its mean $\alpha^3$. The standard optimized cutoff gives a set $\Gamma\subseteq\widehat G$ with

$$
|\Gamma|\leq2\alpha^{-3}
$$

such that the nonnegative function $F=1_A*1_A*1_A$ cannot fall from a maximal value to zero under any shift in $B(\Gamma,\alpha)$. If $x$ maximizes $F$, then

$$
F(x+y)>0
\qquad(y\in B(\Gamma,\alpha)).
$$

The support of a convolution of [indicator functions](../../../measure-theory.md#indicator-function) is the corresponding [sumset](../../../additive-combinatorics.md#sumset), so

$$
\boxed{x+B(\Gamma,\alpha)\subseteq\operatorname{supp}F=A+A+A.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Write $d=|\Gamma|$ and identify each character with a residue $r_j\in\mathbb Z/N\mathbb Z$. Partition the $d$-dimensional torus into $Q^d$ cubes of side $1/Q$, where $Q$ is comparable to $N^{1/d}$. Applying the [pigeonhole principle](../../../algebra.md#pigeonhole-principle) to the points

$$
\left(\frac{kr_1}{N},\ldots,\frac{kr_d}{N}\right),
\qquad 0\leq k\leq Q^d,
$$

gives a nonzero residue $q$ satisfying

$$
\left\|\frac{qr_j}{N}\right\|_{\mathbb R/\mathbb Z}\leq\frac1Q
\qquad(1\leq j\leq d).
$$

Consequently $|e^{2\pi imqr_j/N}-1|\leq\rho$ whenever $|m|\leq\rho Q/(4\pi)$. After allowing for integer parts and the small values of $Q$, this produces the centered [arithmetic progression](../../../arithmetic.md#arithmetic-progression)

$$
\{-Lq,\ldots,0,\ldots,Lq\}\subseteq B(\Gamma,\rho)
$$

of length at least $\frac18\rho N^{1/d}$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Part c gives $x+B(\Gamma,\alpha)\subseteq A+A+A$ with $d=|\Gamma|\leq2\alpha^{-3}$. By the [arithmetic progression in a cyclic Bohr set](../../../additive-combinatorics.md#arithmetic-progression-in-a-cyclic-bohr-set), $B(\Gamma,\alpha)$ contains a centered progression of length at least

$$
\frac18\alpha N^{1/d}
\geq\frac18\alpha N^{\alpha^3/2}.
$$

Its translate by $x$ is the required [arithmetic progression](../../../arithmetic.md#arithmetic-progression) in $A+A+A$.

## 3

↑ **Parent:** [Paper 129](paper-129.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

One standard normalized form of the [Croot-Sisask almost-periodicity theorem](../../../additive-combinatorics.md#croot-sisask-almost-periodicity-theorem) is this. Let $A,S$ be finite subsets of an abelian group with $|A+S|\leq K|A|$, let $q\geq2$, let $0<\epsilon<1$, and let $f$ be a complex function. There is $T\subseteq S$ with

$$
|T|\geq(2K)^{-O(q/\epsilon^2)}|S|
$$

such that every $t\in T-T$ satisfies

$$
\|\tau_t(1_A*f)-1_A*f\|_{L^q}
\leq\epsilon\|1_A\|_{L^1}\|f\|_{L^q}.
$$

For the proof, sample $k=O(q/\epsilon^2)$ independent points of $A$ and approximate $1_A*f$ by the empirical average of the corresponding translates of $f$. A moment inequality bounds the expected $L^q$ error, so many samples are good. The small size of $A+S$ lets a translation and pigeonhole argument find many shifts in $S$ producing the same good approximation. Subtracting two such shifts and applying the [triangle inequality](../../../topological-analysis.md#triangle-inequality) yields the almost periods in $T-T$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Apply the assumed [finite-field character approximation](../../../additive-combinatorics.md#finite-field-character-approximation) with error $\epsilon/2$. We obtain $k\leq4q/\epsilon^2$ characters $\gamma_i$ and a function

$$
P=\frac1k\sum_{i=1}^kc_i\gamma_i\,\|\widehat f\|_{\ell^1}
$$

such that $\|f-P\|_{L^q}\leq(\epsilon/2)\|\widehat f\|_{\ell^1}$. Let

$$
W=\bigcap_{i=1}^k\ker\gamma_i.
$$

Each character has a kernel of codimension at most one, so $\operatorname{codim}W\leq k\leq4q/\epsilon^2$. For $x\in W$, $\tau_xP=P$, and translation invariance of the $L^q$ norm gives

$$
\boxed{\|\tau_xf-f\|_{L^q}
\leq\|\tau_x(f-P)\|_{L^q}+\|f-P\|_{L^q}
\leq\epsilon\|\widehat f\|_{\ell^1}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Put $F=1_A*1_A$. Then $0\leq F\leq1$, $\mathbb EF=\alpha^2$, and the [Parseval identity](../../../fourier-analysis.md#parseval-identity) gives

$$
\|\widehat F\|_{\ell^1}
=\sum_\gamma|\widehat{1_A}(\gamma)|^2
=\alpha.
$$

Set $d=\lfloor\alpha^2n/(8p^2)\rfloor$. If $d<2$, the asserted integer lower bound is trivial. Otherwise take $q=d$ and $\epsilon=3\alpha/(4p)$ in part b. The resulting subspace $W$ has

$$
\operatorname{codim}W
\leq\frac{4d}{\epsilon^2}
=\frac{64p^2d}{9\alpha^2}
\leq\frac{8n}{9}.
$$

Thus $\dim W\geq n/9>d$, and we may choose a $d$-dimensional subspace $D\leq W$.

For $x\in D$, part b gives

$$
\|\tau_xF-F\|_{L^q}
\leq\epsilon\|\widehat F\|_{\ell^1}
=\frac{3\alpha^2}{4p}.
$$

Apply the supplied maximal inequality to $g(x,y)=F(y+x)-F(y)$. Since $|D|^{1/q}=p$, it gives

$$
\mathbb E_y\sup_{x\in D}|F(y+x)-F(y)|
\leq p\frac{3\alpha^2}{4p}
=\frac{3\alpha^2}{4}
<\mathbb EF.
$$

Hence some $y$ satisfies $F(y)>sup_{x\in D}|F(y+x)-F(y)|$, so $F(y+x)>0$ for every $x\in D$. Since $\operatorname{supp}F=A+A$, this proves

$$
\boxed{y+D\subseteq A+A,
\qquad
\dim D\geq\left\lfloor\frac{\alpha^2n}{8p^2}\right\rfloor.}
$$

## 4

↑ **Parent:** [Paper 129](paper-129.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For functions $(f_\epsilon)_{\epsilon\in\{0,1\}^3}$ on $\mathbb F_p^n$, the [Gowers inner product](../../../additive-combinatorics.md#gowers-inner-product) is

$$
\left\langle(f_\epsilon)\right\rangle_{U^3}
=\mathbb E_{x,h_1,h_2,h_3}
\prod_{\epsilon\in\{0,1\}^3}
\mathcal C^{|\epsilon|}f_\epsilon(x+\epsilon_1h_1+\epsilon_2h_2+\epsilon_3h_3),
$$

where $\mathcal C$ is the [complex conjugate](../../../complex-analysis.md#complex-conjugate) operator. The [Gowers uniformity norm](../../../additive-combinatorics.md#gowers-uniformity-norm) is

$$
\|f\|_{U^3}
=\left\langle(f)_{\epsilon\in\{0,1\}^3}\right\rangle_{U^3}^{1/8}.
$$

The [Gowers-Cauchy-Schwarz inequality](../../../additive-combinatorics.md#gowers-cauchy-schwarz-inequality) states

$$
\boxed{\left|\left\langle(f_\epsilon)\right\rangle_{U^3}\right|
\leq\prod_{\epsilon\in\{0,1\}^3}\|f_\epsilon\|_{U^3}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Repeated [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) shows that the $U^3$ norm dominates the absolute mean of a function:

$$
|\mathbb Ef|\leq\|f\|_{U^3}.
$$

Taking $f=1_A$ and using $\mathbb E1_A=\alpha$ gives

$$
\boxed{\|1_A\|_{U^3}\geq\alpha.}
$$

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

For $h(x)=e_p(q(x))$, the product in the $U^3$ cube average is

$$
e_p\!\left(
\sum_{\epsilon\in\{0,1\}^3}(-1)^{|\epsilon|}
q(x+\epsilon\mathbin\cdot h)
\right).
$$

The expression in parentheses is the third additive derivative of the [quadratic form](../../../linear-algebra.md#quadratic-form) $q$, so it vanishes. Every cube contributes one and therefore the [quadratic phase](../../../additive-combinatorics.md#quadratic-phase) satisfies

$$
\boxed{\|h\|_{U^3}=1.}
$$

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Apply the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) successively in the three shift variables to the correlation with the [quadratic phase](../../../additive-combinatorics.md#quadratic-phase) $h$. At the third step the third additive derivative of its phase vanishes, leaving

$$
|\langle f,h\rangle|^8\leq\|f\|_{U^3}^8.
$$

Thus $|\langle f,h\rangle|\geq\delta$ implies

$$
\boxed{\|f\|_{U^3}\geq\delta.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Expand the $U^3$ cube product for

$$
g(x,y)=1_S(x)e_p(\phi(x)^Ty).
$$

Whenever all eight $x$-vertices of the cube lie in $S$, the [Freiman homomorphism](../../../additive-combinatorics.md#freiman-homomorphism) property makes every second additive derivative of $\phi$ vanish. Consequently the coefficients of $y$ and of each of the three $y$-direction increments in the phase cancel, so the phase product around the cube is one. It follows that

$$
\|g\|_{U^3(\mathbb F_p^{n+N})}^8
=\|1_S\|_{U^3(\mathbb F_p^n)}^8.
$$

Part b(i), applied to $S$, now gives

$$
\|g\|_{U^3}\geq\sigma.
$$

Since $|g|\leq1$, one can apply the [inverse theorem for the Gowers U3 norm over a finite field](../../../additive-combinatorics.md#inverse-theorem-for-the-gowers-u3-norm-over-a-finite-field): $g$ has nontrivial correlation, quantitatively in $p$ and $\sigma$, with a [quadratic phase](../../../additive-combinatorics.md#quadratic-phase) on $\mathbb F_p^{n+N}$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
