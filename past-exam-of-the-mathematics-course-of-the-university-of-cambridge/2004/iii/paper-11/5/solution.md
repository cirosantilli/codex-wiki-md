<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $x\in\Omega$ and nonempty $A$, let

$$
U(x,A)=\{(\mathbf1_{x_i\ne y_i})_{i=1}^n:y\in A\},\qquad
V(x,A)=\operatorname{conv}U(x,A).
$$

The [Talagrand convex distance](../../../../../talagrand-convex-distance.md) is

$$
\boxed{d_T(x,A)=\min_{v\in V(x,A)}\|v\|_2.}
$$

Equivalently,

$$
d_T(x,A)=\sup_{\substack{\alpha_i\geq0\\\sum_i\alpha_i^2\leq1}}
\inf_{y\in A}\sum_i\alpha_i\mathbf1_{x_i\ne y_i}.
$$

For completeness, let $v_*$ be a closest point of the finite [convex hull](../../../../../convex-hull.md) to zero. If $v_*\ne0$, minimality gives $v_*\cdot(v-v_*)\geq0$ for every $v\in V$. Taking $\alpha=v_*/\|v_*\|$ proves that the supremum is at least $\|v_*\|$. Conversely each permitted $\alpha$ has $\inf_{v\in V}\alpha\cdot v\leq\alpha\cdot v_*\leq\|v_*\|$ by [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md). The weights are nonnegative because the hull has nonnegative coordinates. If $v_*=0$, both sides are zero. This proves the dual definition used below.

We prove [Talagrand's convex distance inequality](../../../../../talagrand-s-convex-distance-inequality.md) by induction on the number of factors. Write $\Omega=\Omega'\times X_n$, with measure $\mu\otimes\nu$, and $F_A=d_T(\cdot,A)^2$. For a last-coordinate value $z$, let $A_z=\{y':(y',z)\in A\}$. Choose a section $B=A_b$ of largest [probability](../../../../../probability.md) $m=\mu(B)>0$, and put $a_z=\mu(A_z)/m\in[0,1]$. The total [event](../../../../../event.md) [probability](../../../../../probability.md) is $p=\Pr(A)=m\sum_z\nu(z)a_z$.

If $A_z$ has positive [probability](../../../../../probability.md), combine mismatch [vectors](../../../../../vector.md) from $A_z$ and from $B$. A weight $t$ on the second section contributes at most $t$ in the last coordinate. [Convexity](../../../../../convex-function.md) of the squared [Euclidean norm](../../../../../euclidean-norm.md) gives, for every $0\leq t\leq1$,

$$
F_A(x',z)\leq(1-t)F_{A_z}(x')+tF_B(x')+t^2.
$$

The last-coordinate contribution is actually zero if $z=b$, so the displayed upper bound remains valid. [Hölder's inequality](../../../../../holder-s-inequality.md) and the induction hypothesis yield

$$
\begin{aligned}
\mathbb E_{\mu}e^{F_A(x',z)/4}
&\leq e^{t^2/4}
\left(\mathbb E_{\mu}e^{F_{A_z}/4}\right)^{1-t}
\left(\mathbb E_{\mu}e^{F_B/4}\right)^t\\
&\leq m^{-1}e^{t^2/4}a_z^{-(1-t)}.
\end{aligned}
$$

For a zero-probability section use $t=1$ directly, so no division by zero or exponent of an infinite quantity is needed.

The [scalar estimate for Talagrand product induction](../../../../../scalar-estimate-for-talagrand-product-induction.md) is

$$
\inf_{0\leq t\leq1}e^{t^2/4}a^{-(1-t)}\leq2-a
\qquad(0\leq a\leq1).
$$

Here is its proof. For $a>0$ [set](../../../../../set-split.md) $L=-\log a$. If $L\leq1/2$, take $t=2L$; the logarithm of the left expression is $L-L^2$. Put $h(L)=\log(2-e^{-L})-L+L^2$. Then $h(0)=h'(0)=0$ and

$$
h''(L)=2-\frac{2e^L}{(2e^L-1)^2}\geq0,
$$

since $(2u-1)^2-u=(4u-1)(u-1)\geq0$ for $u=e^L\geq1$. Thus $h\geq0$. If $L\geq1/2$, choose $t=1$. The already proved boundary case gives $e^{1/4}\leq2-e^{-1/2}\leq2-a$. The same direct choice covers $a=0$.

Average the resulting section bounds over $z$:

$$
\mathbb Ee^{F_A/4}\leq\frac1m\sum_z\nu(z)(2-a_z)
=\frac{2m-p}{m^2}\leq\frac1p,
$$

where the last inequality is equivalent to $(m-p)^2\geq0$. The induction starts on the zero-coordinate singleton, where every positive-probability [event](../../../../../event.md) is the whole space and the moment is one. Hence

$$
\boxed{\mathbb E\exp\{d_T(X,A)^2/4\}\leq\frac1{\Pr(A)}.}
$$

We assume $\Pr(A)>0$; a zero-probability [event](../../../../../event.md) has no finite right-hand bound to prove. [Markov's inequality](../../../../../markov-inequality.md) also gives

$$
\Pr(A)\Pr(d_T(X,A)\geq u)\leq e^{-u^2/4}.
$$

For the subsequence application, let $L(x)$ be the [longest increasing subsequence](../../../../../longest-increasing-subsequence.md) length for independent sequence coordinates. A witness of length $\ell$ uses only $\ell$ positions. If $L(x)=\ell\geq b$ and $y$ satisfies $L(y)\leq a<b$, at least $\ell-a$ witness positions must change: all unchanged witness positions remain in increasing order. Put weights $1/\sqrt\ell$ on the witness and zero elsewhere. The dual distance definition gives

$$
d_T(x,\{L\leq a\})\geq\frac{\ell-a}{\sqrt\ell}
\geq\frac{b-a}{\sqrt b},
$$

where the latter expression increases with $\ell$ for $a\geq0$. Therefore the [increasing-subsequence certificate concentration](../../../../../increasing-subsequence-certificate-concentration.md) bound is

$$
\boxed{\Pr(L\leq a)\Pr(L\geq b)
\leq e^{-(b-a)^2/(4b)}.}
$$

If the lower [event](../../../../../event.md) has [probability](../../../../../probability.md) zero the conclusion is immediate.

Let $m$ be an integer [median](../../../../../median.md), so $\Pr(L\leq m),\Pr(L\geq m)\geq1/2$. Taking the two thresholds in the bound gives, for $t>0$,

$$
\Pr(L\geq m+t)\leq2e^{-t^2/[4(m+t)]},\qquad
\Pr(L\leq m-t)\leq2e^{-t^2/(4m)}.
$$

For $t>m$ the lower [event](../../../../../event.md) is empty. In a nonempty sequence $m\geq1$. Integration of these tails gives an explicit mean-median estimate: use $m+t\leq2m$ for $t\leq m$ and $m+t\leq2t$ for $t\geq m$, obtaining

$$
|\mathbb EL-m|\leq\mathbb E|L-m|
\leq(\sqrt8+2)\sqrt{\pi m}+16.
$$

Writing $\mu=\mathbb EL$, the [median](../../../../../median.md) property also gives $m\leq2\mu$. Consequently, for a universal constant $C$, all $u\geq0$ satisfy

$$
\boxed{\Pr\{|L-\mu|\geq C(\sqrt\mu+1)+u\}
\leq4\exp\left(-\frac{u^2}{4(2\mu+u)}\right).}
$$

Thus the subsequence length is concentrated near its mean on the scale $\sqrt\mu$, rather than the generic coordinate-exposure scale $\sqrt n$. This argument applies directly to finite-valued independent sequences. Independent continuous samples follow by refining finite coordinate discretizations; the strict-order pattern stabilizes almost surely when ties have [probability](../../../../../probability.md) zero. A uniform random permutation is the rank sequence of independent continuous samples, so it has the same subsequence-length concentration. Arbitrarily dependent random sequences are not covered by the product-space assumption.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
