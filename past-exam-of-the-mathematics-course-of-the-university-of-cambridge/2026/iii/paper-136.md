# Paper 136

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20136.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20136.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
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
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)

## 1

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An [absolute value on a field](../../../arithmetic.md#absolute-value-algebra) is a map $|\cdot|:K\to\mathbb R_{\geq0}$ satisfying $|x|=0\Leftrightarrow x=0$, $|xy|=|x||y|$, and $|x+y|\leq|x|+|y|$. It is [non-Archimedean](../../../arithmetic.md#non-archimedean-absolute-value) when the stronger inequality $|x+y|\leq\max(|x|,|y|)$ holds.

If $\operatorname{char}K=p>0$, then

$$
(x+y)^{p^r}=x^{p^r}+y^{p^r}.
$$

The ordinary triangle inequality gives

$$
|x+y|\leq2^{1/p^r}\max(|x|,|y|).
$$

Letting $r\to\infty$ proves the strong triangle inequality.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

This can be false: take $y=-x\ne0$. Then $|x+y|=0<|x|=\min(|x|,|y|)$. The upper inequality is always the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

This is always true. If, say, $|x|>|y|$, then the ultrametric inequality applied to $x=(x+y)-y$ forces $|x+y|=|x|$; applying it to $x=(x-y)+y$ similarly gives $|x-y|=|x|$.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

This can be false. In a valued field with value group $\mathbb Q$, such as the [Hahn series field](../../../arithmetic.md#hahn-series-field) $k((t^{\mathbb Q}))$, the maximal ideal

$$
\mathfrak m=\{x:v(x)>0\}
$$

of the [valuation ring](../../../commutative-algebra.md#valuation-ring) is not principal: if $v(a)=q>0$, an element of valuation $q/2$ belongs to $\mathfrak m$ but not to $(a)$. Thus the valuation ring need not be a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain).

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

This is always true. Every open ball in an [ultrametric space](../../../arithmetic.md#ultrametric-space) is also closed: a point outside a ball has a disjoint ball of the same radius around it. Distinct points can therefore be separated by clopen sets, so every connected subset is a singleton and $K$ is [totally disconnected](../../../arithmetic.md#totally-disconnected-space).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Two absolute values are equivalent when $|\cdot|_2=|\cdot|_1^c$ for some $c>0$; equivalently, they induce the same topology. The nontrivial non-Archimedean absolute values on $\mathbb Q$ are, up to equivalence, exactly the [p-adic absolute value](../../../arithmetic.md#p-adic-absolute-value) $|\cdot|_p$.

Indeed $|n|\leq1$ for every integer $n$. Nontriviality gives a prime $p$ with $|p|<1$. If $(m,p)=1$, choose $a_r,b_r\in\mathbb Z$ with $a_rm+b_rp^r=1$. For large $r$, $|b_rp^r|<1$, so the ultrametric inequality forces $|m|=1$. Hence

$$
|x|=|p|^{v_p(x)}=|x|_p^c,
\qquad c=-\log_p|p|>0.
$$

If no prime has absolute value below one, the absolute value is trivial. This proves the non-Archimedean part of [Ostrowski theorem](../../../arithmetic.md#ostrowski-s-theorem).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The restriction to $\mathbb Q$ cannot be trivial: otherwise the infinitely many integers would be pairwise distance one inside a bounded ball, contradicting local compactness. By part (c), it induces the $p$-adic topology for one prime $p$. Since a locally compact valued field is complete, the embedding $\mathbb Q\hookrightarrow K$ extends to a closed embedding $\mathbb Q_p\hookrightarrow K$.

Now $K$ is a locally compact topological vector space over the nondiscrete [local field](../../../arithmetic.md#local-field) $\mathbb Q_p$. Such a vector space is finite-dimensional: a compact neighbourhood, together with a maximal linearly independent subset chosen at a fixed separation scale, is totally bounded only if that subset is finite, and its span is then open and closed; maximality makes it all of $K$. Thus $[K:\mathbb Q_p]<\infty$.

## 2

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

One form of [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) is: if $R$ is a complete [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring), $f\in R[X]$, and $f(a_1)\equiv0\pmod\pi$ while $f'(a_1)\not\equiv0\pmod\pi$, then there is a unique $\alpha\in R$ with $f(\alpha)=0$ and $\alpha\equiv a_1\pmod\pi$.

Inductively, if $f(a_n)\equiv0\pmod{\pi^n}$, choose $t$ modulo $\pi$ so that

$$
f(a_n)+\pi^ntf'(a_n)\equiv0\pmod{\pi^{n+1}}
$$

and put $a_{n+1}=a_n+\pi^nt$. The unit $f'(a_n)$ makes $t$ unique. The resulting sequence is Cauchy, so completeness gives a root $\alpha$. Applying the same first-order congruence to two roots proves uniqueness.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $f(X)=X^2-X-2m$, $f(0)\equiv0\pmod2$ and $f'(0)\equiv1\pmod2$. Hensel's lemma gives $x\in\mathbb Z_2$ with $x^2-x=2m$, hence

$$
(2x-1)^2=1+8m.
$$

For $v=\infty$, signs give two square classes and $4/|2|_\infty=2$. For odd $p$, parity of $v_p$ gives two classes and $\mathbb F_p^*/(\mathbb F_p^*)^2$ gives two more, while Hensel makes every unit congruent to $1$ modulo $p$ a square; hence there are four. For $p=2$, valuation parity gives two classes and odd units modulo squares are represented by $1,3,5,7\bmod8$, giving eight. Thus in every case

$$
\boxed{|\mathbb Q_v^*/(\mathbb Q_v^*)^2|=\frac4{|2|_v}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [Laurent series field](../../../arithmetic.md#laurent-series-field) $k((t))$ consists of series $\sum_{n\geq N}a_nt^n$. The map

$$
v_t\left(\sum a_nt^n\right)=\min\{n:a_n\ne0\}
$$

is a discrete valuation. A Cauchy sequence has each coefficient eventually constant, and these stabilized coefficients define its limit, proving completeness.

For $K=\mathbb F_p((t))$, write $K^*=t^{\mathbb Z}\times\mathbb F_p^*\times(1+t\mathbb F_p[[t]])$. If $p$ is odd, Hensel's lemma makes squaring an automorphism of the last factor, so the square-class group has order four. If $p=2$, Frobenius sends $\sum a_nt^n$ to $\sum a_n^2t^{2n}$, and the classes of units with arbitrarily placed odd-degree terms give infinitely many square classes. Hence the group is finite exactly for odd $p$.

## 3

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For sufficiently large $r$, the convergent [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm) and [p-adic exponential](../../../arithmetic.md#p-adic-exponential-function) series are inverse homomorphisms

$$
\log:1+\pi^r\mathcal O_K\longleftrightarrow\pi^r\mathcal O_K:\exp.
$$

Their identities $\log(xy)=\log x+\log y$ and $\exp(x+y)=\exp x\exp y$ follow first formally and then by convergence. Multiplication by $\pi^r$ identifies $(\mathcal O_K,+)$ with $(\pi^r\mathcal O_K,+)$. Since $(1+\pi^r\mathcal O_K)$ has finite index in $\mathcal O_K^*$, the conclusion follows.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Since $\bar a^{q-1}=1$ in the residue field, $u=a^{q-1}\in1+\pi\mathcal O_K$. Powers $u^{q^n}$ tend to one, by the binomial theorem initially and the $p$-adic logarithm once they enter its convergence domain. Therefore $a^{q^n}$ is Cauchy; let its limit be $\omega$. Reduction modulo $\pi$ gives $\bar\omega=\bar a$, while

$$
\omega^{q-1}=\lim_{n\to\infty}u^{q^n}=1.
$$

This is the [Teichmuller representative](../../../arithmetic.md#teichmuller-representative) of $\bar a$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For odd $p$, $\mathbb Q_p$ contains exactly the $p-1$ Teichmuller roots of unity; for $p=2$ it contains $\{\pm1\}$, so there are two. For odd $p$, adjoining $\zeta_p$ adds the $p$ roots of unity of $p$-power order and no primitive $p^2$th root, because the latter would enlarge the degree by $p$. Combining the coprime-order groups gives

$$
|\mu(\mathbb Q_p(\zeta_p))|=p(p-1).
$$

For $p=2$, $\zeta_2=-1$ already lies in $\mathbb Q_2$, so the answer remains two.

## 4

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The residue field $k_K=\mathbb F_q$ has a unique degree-$n$ extension $\mathbb F_{q^n}$. Choose a monic irreducible polynomial $\bar f$ defining it and lift $\bar f$ to a monic $f\in\mathcal O_K[X]$. Hensel's lemma shows that a root generates an unramified extension $L/K$ of degree $n$ with that residue field. Any two such extensions embed into a common algebraic closure and have the same Teichmuller lifts of $\mathbb F_{q^n}$, which generate them; hence they coincide. This proves existence and uniqueness of the [unramified extension](../../../arithmetic.md#unramified-extension).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For $G=\operatorname{Gal}(L/K)$ define

$$
G_0=\ker(G\to\operatorname{Gal}(k_L/k_K)),\qquad
G_i=\{\sigma\in G:v_L(\sigma(\pi_L)-\pi_L)\geq i+1\}\quad(i\geq1).
$$

These are the lower [ramification groups](../../../arithmetic.md#ramification-group). If $\sigma$ lies in every $G_i$, then $\sigma(\pi_L)=\pi_L$; the equivalent definition using all $a\in\mathcal O_L$ then gives $\sigma(a)=a$, so $\sigma=1$.

For $\sigma\in G_0$, set

$$
\theta(\sigma)=\overline{\sigma(\pi_L)/\pi_L}\in k_L^*.
$$

Because inertia acts trivially on $k_L$, $\theta$ is a homomorphism. Its kernel is exactly $G_1$, so it induces an injection $G_0/G_1\hookrightarrow k_L^*$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

The polynomial $X^3-2$ is Eisenstein over $\mathbb Q_2$, hence irreducible. Its discriminant is $-108=36(-3)$, and $-3\equiv5\pmod8$ is not a square in $\mathbb Q_2$. Therefore its splitting field has Galois group $S_3\cong D_6$.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Suppose $G\cong D_{10}$. For residue characteristic two, $G_1$ is a normal $2$-group, $G_0/G_1$ embeds in $k_L^*$, and $G/G_0\cong\operatorname{Gal}(k_L/\mathbb F_2)$ is cyclic. The only proper nontrivial normal subgroup of $D_{10}$ is its rotation subgroup $C_5$, and it has no nontrivial normal $2$-subgroup.

Thus either $G_0=G$ or $G_0=C_5$. In the first case $G_1=1$, so part (b) would embed the noncyclic group $D_{10}$ in the cyclic group $k_L^*$, impossible. In the second case the residue degree is $|G/G_0|=2$, so $k_L=\mathbb F_4$ and $k_L^*$ has order three; it cannot contain the injected group $G_0/G_1=C_5$. Both cases contradict the ramification constraints, so no such extension exists.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
