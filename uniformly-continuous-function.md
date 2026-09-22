# Uniformly continuous function

↑ **Parent:** [Continuous function](continuous-function.md)

A [uniformly continuous function](uniformly-continuous-function.md) has one input tolerance valid throughout its [domain of a function](domain-of-a-function.md). For $f:D\to\mathbb R$, with $D\subseteq\mathbb R$, [uniform continuity](uniform-continuity.md) means

$$
\forall\varepsilon>0\ \exists\delta>0\ \forall x,y\in D:
\quad |x-y|<\delta\ \Longrightarrow\ |f(x)-f(y)|<\varepsilon.
$$

Choose the output tolerance $\varepsilon$ first, then a positive $\delta$ valid for every pair of [function inputs](function-input.md). It may depend on $\varepsilon$, the [function](function-split.md) and its [domain of a function](domain-of-a-function.md), but not on the pair’s location. The [absolute values](absolute-value.md) measure input and output distance.[§3.4, Definition 3.4.1: a single positive input tolerance for all pairs in the specified real domain](basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl.md)

Compare the [quantifier](quantifier.md) order with the [epsilon-delta definition of continuity](epsilon-delta-definition-of-continuity.md):

$$
\begin{aligned}
\text{continuity throughout }D:&\quad
\forall a\in D\ \forall\varepsilon>0\ \exists\delta>0\ \forall x\in D,\\
\text{uniform continuity on }D:&\quad
\forall\varepsilon>0\ \exists\delta>0\ \forall a\in D\ \forall x\in D.
\end{aligned}
$$

Both lines end with $|x-a|<\delta\Rightarrow|f(x)-f(a)|<\varepsilon$. In the first, $\delta$ can depend on the [point](point-geometry.md) $a$; in the second, it is chosen before $a$. Thus [uniform continuity](uniform-continuity.md) implies [continuity](continuous-function.md) at every [point](point-geometry.md). Each requested $\varepsilon$ gets its own shared tolerance.

For an exact example, take the [polynomial function](polynomial-function.md) $f(x)=x^2$ on the [closed interval](closed-real-interval.md) $D=[0,2]$. For every pair of [function inputs](function-input.md) in that [interval](interval-mathematics.md), [polynomial factorization](factorization-of-polynomials.md) gives

$$
|x^2-y^2|=|x-y|\,|x+y|\leq4|x-y|.
$$

Consequently $\delta=\varepsilon/4$ works everywhere on this [domain of a function](domain-of-a-function.md). With $\varepsilon=0.4$, the common tolerance is $\delta=0.1$. Near the right endpoint, for example, $x=1.92$ and $y=2$ have input distance $0.08$ and output distance $4-1.92^2=0.3136<0.4$. The bound is sufficient; it does not claim the largest admissible input window at each [point](point-geometry.md).

On the whole [real line](real-line.md), the same [polynomial function](polynomial-function.md) is a [continuous function](continuous-function.md) but fails [uniform continuity](uniform-continuity.md). Take the [sequences](sequence.md) $x_n=n$ and $y_n=n+1/n$, for positive [integers](integer-split.md) $n$. Then

$$
|x_n-y_n|=\frac1n\longrightarrow0,
\qquad
|x_n^2-y_n^2|=2+\frac1{n^2}>2.
$$

For any proposed $\delta>0$, choose an [integer](integer-split.md) $n>1/\delta$. The inputs are closer than $\delta$, yet their outputs violate the fixed tolerance $\varepsilon=1$. The [sequences](sequence.md) need not themselves have a finite [limit](limit-of-a-function.md): their mutual distance is what tends to zero. This is the obstruction captured by the [sequential criterion for uniform continuity](sequential-criterion-for-uniform-continuity.md). Restricting the [domain of a function](domain-of-a-function.md) to $[0,2]$ removes these escaping pairs.

<a id="image-the-square-function-local-input-windows-shrink-but-a-bounded-interval-admits-one-shared-tolerance"></a>
![](square-uniform-continuity-domains.png)

**[Figure 21](#image-the-square-function-local-input-windows-shrink-but-a-bounded-interval-admits-one-shared-tolerance). The square function: local input windows shrink, but a bounded interval admits one shared tolerance**. The left panel computes sufficient windows $\delta(a)=0.4/(2|a|+1)$ from the [continuity bounds for the square function](continuity-bounds-for-the-square-function.md); shrinking these particular windows alone does not prove failure of [uniform continuity](uniform-continuity.md). The middle panel displays the exact bound $4|x-y|$ on the [interval](interval-mathematics.md) $[0,2]$. The right panel gives the decisive [sequence](sequence.md) pairs $n,n+1/n$ on the [real line](real-line.md). All plotted values are calculated from the displayed formulas.

A [uniformly continuous function](uniformly-continuous-function.md) need not be a [bounded function](bounded-function.md). The [identity function](identity-function.md) $f(x)=x$ on the [real line](real-line.md) has $|f(x)-f(y)|=|x-y|$, so $\delta=\varepsilon$ always works, although its [image of a function](image-of-a-function.md) is the unbounded [real line](real-line.md). [Uniform continuity](uniform-continuity.md) controls changes between nearby inputs, not the overall size of outputs. Likewise, an unbounded [domain of a function](domain-of-a-function.md) does not by itself prevent [uniform continuity](uniform-continuity.md).

The [square root](square-root.md) $g(x)=\sqrt x$ supplies a different common tolerance on the [interval](interval-mathematics.md) $[0,\infty)$. Assuming $x\geq y\geq0$, put $u=\sqrt x$ and $v=\sqrt y$. Since $0\leq u-v\leq u+v$,

$$
(u-v)^2\leq(u-v)(u+v)=x-y.
$$

Interchanging the inputs when necessary proves

$$
|\sqrt x-\sqrt y|\leq\sqrt{|x-y|}.
$$

Thus $\delta=\varepsilon^2$ guarantees [uniform continuity](uniform-continuity.md) on the entire [domain of a function](domain-of-a-function.md), including zero. For $\varepsilon=0.4$, any input distance below $0.16$ suffices. The pairs $(0,0.09)$ and $(4,4.09)$ both have input distance $0.09$; their output distances are respectively $0.3$ and $0.09/(\sqrt{4.09}+2)<0.0225$. The common guarantee accommodates quite different local sensitivities.

This [Hölder continuity](holder-condition.md) bound allows a curved tolerance rule. It is weaker than a [Lipschitz bound](lipschitz-bound.md): at zero the output change divided by the input change is

$$
\frac{|g(h)-g(0)|}{|h-0|}=\frac1{\sqrt h}\longrightarrow\infty
\qquad(h\downarrow0).
$$

No finite [Lipschitz constant](lipschitz-constant.md) works near zero, even though [uniform continuity](uniform-continuity.md) does. A [Lipschitz function](lipschitz-continuity.md) does have [uniform continuity](uniform-continuity.md), choosing $\delta=\varepsilon/L$ when its [Lipschitz bound](lipschitz-bound.md) $L$ is positive; when $L=0$ it is a [constant function](constant-function.md).[§3.4, Proposition 3.4.8 and Example 3.4.10: Lipschitz continuity implies uniform continuity; the square root on the nonnegative half-line separates the properties](basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl.md)

<a id="image-square-root-input-changes-share-an-output-tolerance-even-though-amplification-near-zero-is-unbounded"></a>
![](square-root-uniform-tolerance.png)

**[Figure 22](#image-square-root-input-changes-share-an-output-tolerance-even-though-amplification-near-zero-is-unbounded). Square-root input changes share an output tolerance even though amplification near zero is unbounded**. At left, the exact output changes $\sqrt{a+h}-\sqrt a$ for base [points](point-geometry.md) $a=0,1,4$ stay inside $\varepsilon=0.4$ whenever $|h|<\delta=0.16$ and $a+h\geq0$. The right panel computes the amplification $1/\sqrt h$ for inputs $0,h$: it grows without bound as $h$ decreases. These are calculated [function graphs](graph-of-a-function.md), with no experimental measurements.

For general [metric spaces](metric-space.md), replace the [absolute values](absolute-value.md) by the respective [distance functions](metric.md). The [Heine-Cantor theorem](heine-cantor-theorem.md) gives an existence guarantee: every [continuous function](continuous-function.md) on a [compact metric space](compact-metric-space.md) is [uniformly continuous](uniform-continuity.md). In particular, [continuity](continuous-function.md) on a finite [closed interval](closed-real-interval.md) provides a common tolerance, even when no simple formula for it is known.[§7.5, Definition 7.5.10 and Theorem 7.5.11: uniform continuity between metric spaces and the compact-domain theorem](basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl.md)

For a short proof outline, fix $\varepsilon>0$. [Continuity](continuous-function.md) gives each [point](point-geometry.md) $a$ an [open ball](open-ball.md) of radius $r_a>0$ within which outputs differ from $f(a)$ by less than $\varepsilon/2$. The [open balls](open-ball.md) of half these radii still cover the [domain of a function](domain-of-a-function.md). [Compactness](compact-space.md) supplies a [finite subcover](finite-subcover.md). Take $\delta$ to be the smallest half-radius in this [finite set](finite-set.md). Two inputs closer than $\delta$ lie together in one of the original [open balls](open-ball.md), so the [triangle inequality](triangle-inequality.md) bounds their output distance by $\varepsilon$. The beautiful step is that the [compact set](compact-space.md) turns local choices into finitely many choices, whose minimum stays positive.

A shared tolerance also makes [uniformly continuous functions](uniformly-continuous-function.md) preserve [Cauchy sequences](cauchy-sequence.md): after choosing $\delta$ for $\varepsilon$, all sufficiently late input pairs are closer than $\delta$, so all corresponding output pairs are closer than $\varepsilon$. Unlike a [convergent sequence](convergent-sequence.md) argument, this does not require an input [limit](limit-of-a-function.md) inside the [domain of a function](domain-of-a-function.md). It is why [uniform continuity](uniform-continuity.md) is useful for extending a [function](function-split.md) toward missing endpoints and for the decay argument below.

**Table of contents**

- [Decay of a nonnegative uniformly continuous integrable function](decay-of-a-nonnegative-uniformly-continuous-integrable-function.md)

## ↑ Ancestors (8)

1. [Continuous function](continuous-function.md)
2. [Limit of a function](limit-of-a-function.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Decay of a nonnegative uniformly continuous integrable function](decay-of-a-nonnegative-uniformly-continuous-integrable-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29/4/i/solution.md)
- [Uniformly continuous function](uniformly-continuous-function.md)
- [Uniformly continuous integrable functions vanish at infinity](uniformly-continuous-integrable-functions-vanish-at-infinity.md)
