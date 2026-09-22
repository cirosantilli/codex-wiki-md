# Paper 129

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_129.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_129.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
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
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)

## 1

↑ **Parent:** [Paper 129](paper-129.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For every $x\in BC^{-1}$, choose one representation $x=b_xc_x^{-1}$. Define

$$
F:A\times BC^{-1}\longrightarrow AB^{-1}\times AC^{-1},
\qquad
F(a,x)=(ab_x^{-1},ac_x^{-1}).
$$

The image determines

$$
(ab_x^{-1})^{-1}(ac_x^{-1})=b_xc_x^{-1}=x,
$$

and the chosen representative then determines $a=(ab_x^{-1})b_x$. Thus $F$ is injective, and counting its domain and codomain proves the [Noncommutative Ruzsa triangle inequality](../../../additive-combinatorics.md#noncommutative-ruzsa-triangle-inequality)

$$
\boxed{|A|\,|BC^{-1}|\leq|AB^{-1}|\,|AC^{-1}|.}
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Choose $a_0\in A$. Right multiplication by $a_0$ injects $A^2$ into $A^3$, so

$$
|A^2|\leq|A^3|\leq K|A|.
$$

Apply part i with anchor $A^{-1}$, $B=A$, and $C=A^2$. Since inversion preserves cardinality,

$$
|A|\,|AA^{-1}A^{-1}|
\leq |A^{-1}A^{-1}|\,|A^{-1}A^{-1}A^{-1}|
=|A^2|\,|A^3|
\leq K^2|A|^2.
$$

Therefore $|AA^{-1}A^{-1}|\leq K^2|A|$.

Apply part i again, now with anchor $A$, $B=A^2$, and $C=A^{-1}A^{-1}$. This gives

$$
|A|\,|A^4|
\leq|AA^{-1}A^{-1}|\,|A^3|
\leq K^3|A|^2.
$$

**Thus $|A^4|\leq K^3|A|$. Since $K\geq1$, this proves the requested [fourfold product bound from small tripling](../../../additive-combinatorics.md#fourfold-product-bound-from-small-tripling) $|A^4|\leq K^4|A|$.**

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Let $H$ be a finite group and form the [free product](../../../algebraic-topology.md#free-product) $G=H*\langle x\rangle$. Put $A=H\cup\{x\}$. Then

$$
A^2\subseteq H\cup Hx\cup xH\cup\{x^2\},
$$

so $|A^2|\leq3|H|+1<3|A|$.

On the other hand, $A^3$ contains the double coset $HxH$. Reduced-word uniqueness in the free product makes the map

$$
H\times H\longrightarrow HxH,
\qquad(h_1,h_2)\longmapsto h_1xh_2
$$

injective, so $|A^3|\geq|H|^2$. Taking finite groups $H$ of unbounded order keeps the doubling constant below three while $|A^3|/|A|$ tends to infinity. This realizes the [small doubling does not control tripling in a noncommutative group](../../../additive-combinatorics.md#small-doubling-does-not-control-tripling-in-a-noncommutative-group) phenomenon.

## 2

↑ **Parent:** [Paper 129](paper-129.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Take $x_1,x_2,x_3,x_4\in\phi^{-1}(W)$ with $x_1+x_2=x_3+x_4$. Write $x_3=x_1+a$ and $x_4=x_1+b$; then $x_2=x_1+a+b$. Hence

$$
D=\phi(x_1)-\phi(x_3)-\phi(x_4)+\phi(x_2)
$$

belongs to $X$. All four values of $\phi$ lie in the same affine subspace $W=V+w$, and their coefficients in $D$ sum to zero, so $D\in V$. The hypothesis $V\cap X=\{0\}$ gives $D=0$, precisely the additive-quadruple identity required of a [Freiman homomorphism](../../../additive-combinatorics.md#freiman-homomorphism). This is the [second-difference obstruction to a Freiman homomorphism](../../../additive-combinatorics.md#second-difference-obstruction-to-a-freiman-homomorphism).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let $G_0=\mathbb F_p^n$ and let

$$
\Gamma=\{(x,\phi(x)):x\in G_0\}\subseteq G_0\times G_0.
$$

For each fixed first coordinate $d$, the second coordinates occurring in $\Gamma-\Gamma$ are values of $\phi(x+d)-\phi(x)$, of which there are at most $C$. Therefore

$$
|\Gamma-\Gamma|\leq C|G_0|=C|\Gamma|.
$$

The difference-set form of the [Plünnecke-Ruzsa inequality](../../../additive-combinatorics.md#plunnecke-ruzsa-inequality) now gives

$$
|3\Gamma-2\Gamma|\leq C^5|\Gamma|.
$$

Every $u\in X$ has the form

$$
(0,u)=(x,\phi(x))-(x+a,\phi(x+a))-(x+b,\phi(x+b))+(x+a+b,\phi(x+a+b)),
$$

so $\{0\}\times X\subseteq2\Gamma-2\Gamma$. Consequently

$$
(\{0\}\times X)+\Gamma\subseteq3\Gamma-2\Gamma.
$$

The set on the left has exactly $|X||\Gamma|$ elements, since its fiber over each $x$ is $\phi(x)+X$. It follows that

$$
|X||\Gamma|\leq C^5|\Gamma|,
$$

and hence $|X|\leq C^5$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Choose $k$ so that

$$
|X|\leq p^k<p|X|
$$

and take a uniformly random codimension-$k$ subspace $V\leq\mathbb F_p^n$. Each fixed nonzero vector lies in $V$ with probability at most $p^{-k}$. The [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\mathbb P((X\setminus\{0\})\cap V\ne\varnothing)
\leq(|X|-1)p^{-k}<1.
$$

Thus some $V$ satisfies $V\cap X=\{0\}$.

For a uniformly random coset $W$ of this $V$, every value $\phi(x)$ lies in $W$ with probability $p^{-k}$. Therefore

$$
\mathbb E_W|\phi^{-1}(W)|=p^{-k}p^n,
$$

so some coset has inverse image $A$ of density at least

$$
p^{-k}>\frac1{p|X|}\geq p^{-1}C^{-5}.
$$

Part i says that $\phi|_A$ is a Freiman homomorphism, proving the [large Freiman-homomorphic restriction from bounded derivative images](../../../additive-combinatorics.md#large-freiman-homomorphic-restriction-from-bounded-derivative-images).

## 3

↑ **Parent:** [Paper 129](paper-129.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The finite-field [Bogolyubov lemma](../../../additive-combinatorics.md#bogolyubov-lemma) states that if $A\subseteq G=\mathbb F_p^n$ has density $\alpha$, then $2A-2A$ contains a subspace of codimension at most $2\alpha^{-2}$.

Use normalized [Fourier analysis on a finite abelian group](../../../additive-combinatorics.md#normalized-fourier-analysis-on-a-finite-abelian-group) and put $f=1_A$. Define

$$
S=\left\{\gamma\in\widehat G:|\widehat f(\gamma)|\geq\frac{\alpha^{3/2}}{\sqrt2}\right\}.
$$

By [Parseval identity](../../../fourier-analysis.md#parseval-identity),

$$
|S|\frac{\alpha^3}{2}\leq\sum_\gamma|\widehat f(\gamma)|^2=\alpha,
$$

so $|S|\leq2\alpha^{-2}$. Let

$$
V=\{x\in G:\gamma(x)=1\text{ for every }\gamma\in S\}.
$$

Then $V$ is a subspace of codimension at most $|S|$.

The normalized representation function of $2A-2A$ is

$$
r(x)=(f*f*\widetilde f*\widetilde f)(x)
=\sum_{\gamma\in\widehat G}|\widehat f(\gamma)|^4\gamma(x),
$$

where $\widetilde f(x)=f(-x)$. For $x\in V$, all terms indexed by $S$ are nonnegative real numbers, while

$$
\sum_{\gamma\notin S}|\widehat f(\gamma)|^4
\leq\frac{\alpha^3}{2}\sum_\gamma|\widehat f(\gamma)|^2
=\frac{\alpha^4}{2}.
$$

The trivial character alone contributes $\alpha^4$, so $r(x)>0$. Hence $x\in2A-2A$, proving the [Finite-field Bogolyubov lemma](../../../additive-combinatorics.md#finite-field-bogolyubov-lemma).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The hypothesis says that the [additive energy](../../../additive-combinatorics.md#additive-energy) satisfies $E(A)\geq c|A|^3$. The [Balog-Szemerédi-Gowers theorem](../../../additive-combinatorics.md#balog-szemeredi-gowers-theorem) supplies $A'\subseteq A$ with

$$
|A'|\geq c_1(c)|A|,
\qquad
|A'+A'|\leq C_1(c)|A'|.
$$

By the [Freiman-Ruzsa theorem over a finite field](../../../additive-combinatorics.md#freiman-ruzsa-theorem-over-a-finite-field), $A'$ lies in a subspace $H$ with

$$
|H|\leq C_2(c,p)|A'|.
$$

Thus $A'$ has density at least $C_2^{-1}$ in $H$. Applying the [Finite-field Bogolyubov lemma](../../../additive-combinatorics.md#finite-field-bogolyubov-lemma) inside $H$ gives a subspace

$$
V\subseteq2A'-2A'\subseteq2A-2A
$$

of codimension bounded in terms of $c,p$ alone. Therefore

$$
|V|\geq c'(c,p)|H|\geq c'(c,p)|A|,
$$

which is the [additive energy produces a large subspace in a fourfold difference set](../../../additive-combinatorics.md#additive-energy-produces-a-large-subspace-in-a-fourfold-difference-set) result.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [Ruzsa triangle inequality](../../../additive-combinatorics.md#ruzsa-triangle-inequality) applied to $A-A$ also bounds $|A+A|$ in terms of $C|A|$, so $A$ has bounded doubling. The [Freiman-Ruzsa theorem](../../../additive-combinatorics.md#freiman-ruzsa-theorem) places $A$ inside a proper coset progression $P$ whose rank and ratio $|P|/|A|$ are bounded only in terms of $C$. Hence $A$ has positive density bounded in terms of $C$ inside a bounded-rank progression.

For sufficiently large $|A|$, the [Szemerédi theorem in a bounded-rank coset progression](../../../additive-combinatorics.md#szemeredi-theorem-in-a-bounded-rank-coset-progression) gives a nontrivial three-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression) in $A$. This proves the [small difference set forces a three-term arithmetic progression](../../../additive-combinatorics.md#small-difference-set-forces-a-three-term-arithmetic-progression) assertion.

## 4

↑ **Parent:** [Paper 129](paper-129.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

With normalized averages on the finite abelian group $G$, the [Gowers U2 norm](../../../additive-combinatorics.md#gowers-u2-norm) is defined by

$$
\|f\|_{U^2}^4
=\mathbb E_{x,a,b}f(x)\overline{f(x+a)}\,\overline{f(x+b)}f(x+a+b).
$$

The [Gowers U3 norm](../../../additive-combinatorics.md#gowers-u3-norm) is defined by

$$
\|f\|_{U^3}^8
=\mathbb E_{x,a,b,c}
\prod_{\epsilon\in\{0,1\}^3}
\mathcal C^{|\epsilon|}f(x+\epsilon_1a+\epsilon_2b+\epsilon_3c),
$$

where $\mathcal C$ denotes complex conjugation.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Write

$$
\Lambda_4(f_1,f_2,f_3,f_4)
=\mathbb E_{x,d}f_1(x)f_2(x+d)f_3(x+2d)f_4(x+3d).
$$

Apply the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) first in the variable carrying $f_1$ and then in the variable carrying $f_2$. After the invertible linear changes of variables permitted by $2,3\nmid|G|$, apply the assumed three-function $U^2$ estimate to the resulting multiplicative derivatives. The standard calculation gives

$$
|\Lambda_4|^8
\leq\|f_1\|_2^8\|f_2\|_2^8
\left(\mathbb E_h\|\partial_hf_3\|_{U^2}^4\right)
\left(\mathbb E_h\|\partial_hf_4\|_{U^2}^4\right).
$$

By the [Derivative identity for the Gowers U3 norm](../../../additive-combinatorics.md#derivative-identity-for-the-gowers-u3-norm), the last two factors are $\|f_3\|_{U^3}^8$ and $\|f_4\|_{U^3}^8$. Taking eighth roots proves

$$
|\Lambda_4(f_1,f_2,f_3,f_4)|
\leq\|f_1\|_2\|f_2\|_2\|f_3\|_{U^3}\|f_4\|_{U^3}.
$$

If $A\subseteq G$ has density $\alpha$, write $1_A=\alpha+f$. Expanding $\Lambda_4(1_A,1_A,1_A,1_A)$, the constant term is $\alpha^4$, and the displayed inequality bounds every nonconstant term after translation of one factor by a $U^3$ norm of the balanced function $f$. Thus sufficiently small $\|1_A-\alpha\|_{U^3}$ makes the normalized number of four-term [arithmetic progressions](../../../arithmetic.md#arithmetic-progression) close to $\alpha^4$.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Put $M(a)=\max_{\gamma\in\widehat G}|\widehat{\partial_af}(\gamma)|^2$. By the [Derivative identity for the Gowers U3 norm](../../../additive-combinatorics.md#derivative-identity-for-the-gowers-u3-norm), the Fourier formula for the $U^2$ norm, and [Parseval identity](../../../fourier-analysis.md#parseval-identity),

$$
c\leq\mathbb E_a\sum_\gamma|\widehat{\partial_af}(\gamma)|^4
\leq\mathbb E_a M(a)\sum_\gamma|\widehat{\partial_af}(\gamma)|^2
\leq\mathbb E_aM(a),
$$

because $\|f\|_\infty\leq1$. Let

$$
B=\{a:M(a)\geq c/2\},
$$

and for every $a\in B$ choose $\phi(a)\in\widehat G$ attaining $M(a)$. Then

$$
|\widehat{\partial_af}(\phi(a))|^2\geq c/2
$$

for every $a\in B$, and deleting the complement of $B$ from the preceding average leaves total mass at least $c/2$.

Let $\Gamma_\phi=\{(a,\phi(a)):a\in B\}\subseteq G\times\widehat G$. The box-norm inequality applied to the selected Fourier coefficients and the cocycle identity for multiplicative derivatives gives

$$
\left(\mathbb E_a1_B(a)|\widehat{\partial_af}(\phi(a))|^2\right)^8
\leq\frac{E(\Gamma_\phi)}{|G|^3}.
$$

The left side is at least $(c/2)^8$. An additive quadruple in $\Gamma_\phi$ is exactly a tuple $(a,b,c,d)\in B^4$ satisfying

$$
a+b=c+d,
\qquad
\phi(a)\phi(b)=\phi(c)\phi(d).
$$

**Therefore there are at least $(c/2)^8|G|^3$ such quadruples, which is the [Frequency graph extracted from a large Gowers U3 norm](../../../additive-combinatorics.md#frequency-graph-extracted-from-a-large-gowers-u3-norm).**

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Let $A\subseteq\mathbb F_5^n$ have density at least $\delta$ and put $f=1_A-\mathbb E1_A$. If $A$ has too few four-term progressions, part ii forces $\|f\|_{U^3}$ to be large. Part iii then produces a frequency graph with large [additive energy](../../../additive-combinatorics.md#additive-energy). The [Balog-Szemerédi-Gowers theorem](../../../additive-combinatorics.md#balog-szemeredi-gowers-theorem) extracts a large piece with small doubling, and a finite-field Freiman theorem makes the frequency selection approximately affine-linear there. Integrating these approximately linear derivative frequencies produces correlation of $f$ with a [quadratic phase](../../../additive-combinatorics.md#quadratic-phase), as in the [inverse theorem for the Gowers U3 norm over a finite field](../../../additive-combinatorics.md#inverse-theorem-for-the-gowers-u3-norm-over-a-finite-field).

Restricting to a suitable level set of that quadratic phase produces a density increment on a structured affine subspace. Iterating these increments cannot continue indefinitely because density is at most one. Once $n$ is sufficiently large in terms of $\delta$, the iteration must instead terminate with the expected nontrivial four-term progression. This is the [density-increment proof of the finite-field four-term progression theorem](../../../additive-combinatorics.md#density-increment-proof-of-the-finite-field-four-term-progression-theorem).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
