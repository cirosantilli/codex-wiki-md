<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Start with a finite subcover of the [compact set](../../../../../compact-space.md) $K$. Among its remaining [open balls](../../../../../open-ball.md), retain one of greatest radius and discard every ball intersecting it. Repeat until no balls remain. The retained family $\mathcal F$ is finite and pairwise disjoint. If a discarded ball $B(c,r)$ met the retained ball $B(c_0,R)$, then $r\le R$ and $|c-c_0|<r+R$. Therefore, for any $y\in B(c,r)$,

$$
|y-c_0|\le |y-c|+|c-c_0|<2r+R\le3R.
$$

Every original ball lies in the concentric triple of one retained ball. This proves the [Wiener covering lemma](../../../../../wiener-covering-lemma.md) for the finite subcover. By [Lebesgue measure](../../../../../lebesgue-measure.md) scaling and subadditivity,

$$
\lambda_d(K)\le\sum_{B\in\mathcal F}\lambda_d(3B)
=3^d\sum_{B\in\mathcal F}\lambda_d(B).
$$

Disjointness gives

$$
\boxed{\lambda_d\left(\bigcup_{B\in\mathcal F}B\right)
\ge3^{-d}\lambda_d(K).}
$$

The empty [compact set](../../../../../compact-space.md) is covered by the empty selection.

The [spherical derivative of a measure](../../../../../spherical-derivative-of-a-measure.md) at $x$ is the limit

$$
D_s\mu(x)=\lim_{r\downarrow0}
\frac{\mu(B(x,r))}{\lambda_d(B(x,r))}
=\lim_{r\downarrow0}\frac{\mu(B(x,r))}{v_dr^d},
$$

when it exists, where $v_d$ is the unit-ball volume. We prove that this limit is zero outside a Lebesgue-[null set](../../../../../null-set.md) for the singular [measure](../../../../../measure.md).

First derive the needed maximal estimate from the selection lemma. For a finite positive [Borel measure](../../../../../borel-measure.md) $\eta$, put

$$
M_u\eta(x)=\sup_{\substack{B\text{ an open ball}\\x\in B}}
\frac{\eta(B)}{\lambda_d(B)}.
$$

This is the [uncentered maximal function of a finite measure](../../../../../uncentered-maximal-function-of-a-finite-measure.md). For $\alpha>0$, its strict superlevel set is the union of all balls with $\eta(B)>\alpha\lambda_d(B)$, so it is open. Cover any [compact subset](../../../../../compact-space.md) $H$ of this set by such balls and apply the finite [Wiener covering lemma](../../../../../wiener-covering-lemma.md). The selected disjoint balls give

$$
\lambda_d(H)\le3^d\sum_{B\in\mathcal F}\lambda_d(B)
\le\frac{3^d}{\alpha}\sum_{B\in\mathcal F}\eta(B)
\le\frac{3^d}{\alpha}\eta(\mathbb R^d).
$$

By [inner regularity of Lebesgue measure](../../../../../inner-regularity-of-lebesgue-measure.md), this proves the [uncentered maximal weak-type inequality](../../../../../uncentered-maximal-weak-type-inequality.md)

$$
\boxed{\lambda_d\{M_u\eta>\alpha\}
\le\frac{3^d}{\alpha}\eta(\mathbb R^d).}
$$

Since $\mu$ and $\lambda_d$ are [mutually singular measures](../../../../../mutually-singular-measures.md), there is a Borel set $N$ with $\lambda_d(N)=0$ and $\mu(\mathbb R^d\setminus N)=0$. By [regularity of finite Borel measures on Euclidean space](../../../../../regularity-of-finite-borel-measures-on-euclidean-space.md), for each $\varepsilon>0$ choose compact $L\subset N$ with $\mu(\mathbb R^d\setminus L)<\varepsilon$. Define the remainder [measure](../../../../../measure.md) $\eta_\varepsilon(A)=\mu(A\setminus L)$.

For $x\notin L$, distance from $x$ to this [compact set](../../../../../compact-space.md) is positive. Thus sufficiently small centered balls avoid $L$, and

$$
\mu(B(x,r))=\eta_\varepsilon(B(x,r))
\quad\text{for all sufficiently small }r.
$$

Write $\overline D_s\mu(x)$ for the upper limit of the ratios. If it exceeds $\alpha$, then either $x\in L$ or $M_u\eta_\varepsilon(x)>\alpha$. Hence

$$
\{\overline D_s\mu>\alpha\}
\subset L\cup\{M_u\eta_\varepsilon>\alpha\}.
$$

The right side has [Lebesgue measure](../../../../../lebesgue-measure.md) at most $3^d\varepsilon/\alpha$, since $\lambda_d(L)=0$. This even bounds the [outer measure](../../../../../outer-measure.md) of the left side, without a separate measurability argument for the upper density. Let $\varepsilon\downarrow0$, and then take the countable union over positive rational $\alpha$. We obtain $\overline D_s\mu=0$ Lebesgue almost everywhere. The ratios are nonnegative, so their lower limit is also zero and

$$
\boxed{D_s\mu(x)=0\qquad\lambda_d\text{-almost everywhere}.}
$$

This proves that the [spherical derivative of a singular measure vanishes](../../../../../spherical-derivative-of-a-singular-measure-vanishes.md). It is important to approximate the null carrier by [compact subsets](../../../../../compact-space.md): a null carrier can be dense, so points outside it need not have any neighbourhood avoiding it.

In one dimension, consider the [cumulative distribution function](../../../../../cumulative-distribution-function.md) $F$. For either sign of $h\ne0$, monotonicity gives a nonnegative difference quotient, and the relevant half-open interval lies inside $B(x,2|h|)$. In detail, the numerator is $\mu((x,x+h])$ for $h>0$, while after reversing both signs it is $\mu((x+h,x])$ for $h<0$. Thus

$$
0\le\frac{F(x+h)-F(x)}h
\le\frac{\mu(B(x,2|h|))}{|h|}
=4\,\frac{\mu(B(x,2|h|))}{\lambda_1(B(x,2|h|))}.
$$

At each point where the [spherical derivative of a measure](../../../../../spherical-derivative-of-a-measure.md) is zero, this bound tends to zero from both sides. The enlarged open interval avoids any endpoint ambiguity from atoms. Therefore **the ordinary two-sided [derivative](../../../../../derivative.md) exists and**

$$
\boxed{F'(x)=0\qquad\lambda_1\text{-almost everywhere}.}
$$

This is why [singular distribution functions have zero derivative almost everywhere](../../../../../singular-distribution-functions-have-zero-derivative-almost-everywhere.md) without having to be constant: almost-everywhere differentiation recovers increments only under extra hypotheses such as [absolute continuity of a function](../../../../../absolutely-continuous-function.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
