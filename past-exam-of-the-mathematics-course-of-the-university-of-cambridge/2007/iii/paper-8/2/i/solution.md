<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $C=\|T\|$. We construct the extension by a deterministic recursion over the given dense list, using the [one-dimensional dominated extension of a real linear functional](../../../../../../one-dimensional-dominated-extension-of-a-real-linear-functional.md). Neither [Zorn's lemma](../../../../../../zorn-s-lemma.md) nor any selection of a family of extensions is needed.

Suppose $f:W\to\mathbb R$ is already a [linear functional](../../../../../../linear-functional.md) satisfying $|f(w)|\le C\|w\|$, and $v\notin W$. An extension to $W+\mathbb Rv$ must have the form

$$
f_v(w+tv)=f(w)+t a.
$$

Define

$$
L_v=\sup_{w\in W}\bigl(f(w)-C\|w-v\|\bigr),\qquad
U_v=\inf_{w\in W}\bigl(C\|w+v\|-f(w)\bigr).
$$

For any $w,z\in W$, the bound on $f$ and the triangle inequality give

$$
f(w)+f(z)=f(w+z)\le C\|w+z\|\le C\|w-v\|+C\|z+v\|.
$$

Thus every quantity in the supremum defining $L_v$ is at most every quantity in the infimum defining $U_v$. Taking $w=0$ and $z=0$ gives finite bounds, specifically

$$
-C\|v\|\le L_v\le U_v\le C\|v\|.
$$

The completeness of the real numbers defines these endpoints uniquely. Set $a=L_v$; this is an explicit rule, not an arbitrary choice from a nonempty interval.

For $t>0$, the upper-endpoint inequality with $w/t$ yields $f(w)+ta\le C\|w+tv\|$. For $t<0$, write $t=-s$ with $s>0$ and use the lower-endpoint inequality with $w/s$ to obtain the same bound. For $t=0$ it is the original bound. Applying the upper bound also to the negative of the vector gives

$$
|f_v(w+tv)|\le C\|w+tv\|.
$$

The representation $w+tv$ is unique because $v\notin W$, so $f_v$ is a well-defined bounded [linear functional](../../../../../../linear-functional.md) extending $f$.

Start with $W_0=U$ and $f_0=T$. At step $n$, if $y_n\in W_{n-1}$ leave the functional unchanged; otherwise use exactly the supremum-endpoint rule with $v=y_n$. Put $W_n=U+\operatorname{span}\{y_1,\ldots,y_n\}$. This defines compatible functionals $f_n$ on $W_n$ with the common bound $C$. Their union $f_\infty$ on $W_\infty=\bigcup_nW_n$ is linear and bounded by $C$. The subspace $W_\infty$ is dense in $V$ because it contains every $y_n$.

To make the final passage to the closure equally free of the [axiom of choice](../../../../../../axiom-of-choice.md), for $v\in V$ let $j_n(v)$ be the least positive integer with $\|y_{j_n(v)}-v\|<2^{-n}$. Density ensures that this integer exists, and leastness specifies it uniquely. Define

$$
\widetilde T(v)=\lim_{n\to\infty}f_\infty(y_{j_n(v)}).
$$

The limit exists because

$$
|f_\infty(y_{j_n(v)})-f_\infty(y_{j_m(v)})|
\le C(2^{-n}+2^{-m}).
$$

Any other approximating sequence in $W_\infty$ gives the same limit, by the same norm bound. Applying this independence to sums and scalar multiples of approximating sequences proves [linearity](../../../../../../linearity.md) of $\widetilde T$. It also shows $\widetilde T=f_\infty$ on $W_\infty$ and $|\widetilde T(v)|\le C\|v\|$. Restriction to $U$ therefore gives

$$
\boxed{\widetilde T|_U=T,\qquad\|\widetilde T\|=\|T\|.}
$$

The upper bound follows from construction and the lower bound from restriction to $U$. This also covers $C=0$, when all extensions are zero. No completeness of $V$ or closedness of $U$ was assumed. The argument establishes the [choice-free Hahn-Banach extension in a separable space](../../../../../../choice-free-hahn-banach-extension-in-a-separable-space.md) by uniquely specified operations at every stage.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
