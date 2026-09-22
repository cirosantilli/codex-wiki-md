<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $\log^+x=\max(0,\log x)$. The [Nevanlinna proximity function](../../../../../nevanlinna-proximity-function.md) and [Nevanlinna integrated counting function](../../../../../nevanlinna-integrated-counting-function.md) are

$$
m(r,f)=\frac1{2\pi}\int_0^{2\pi}\log^+|f(re^{i\theta})|\,d\theta,
\qquad
N(r,f)=\sum_{|p_n|<r}\log\frac r{|p_n|}.
$$

The pole sum counts [multiplicity](../../../../../multiplicity-mathematics.md); it is finite for each $r$ because $f(0)$ is finite and nonzero and [poles](../../../../../pole.md) of a [meromorphic function](../../../../../meromorphic-function.md) are isolated. Equivalently $N(r,f)=\int_0^r n(t,f)\,dt/t$, where $n(t,f)$ counts poles in the disc. The [Nevanlinna characteristic](../../../../../nevanlinna-characteristic.md) is

$$
\boxed{T(r,f)=m(r,f)+N(r,f).}
$$

For a general nonzero [meromorphic function](../../../../../meromorphic-function.md) $g$ with signed order $\nu$ at zero, use $g(z)=cz^\nu(1+O(z))$, $c\ne0$. The general counting convention includes a pole at zero:

$$
N(r,g)=n(0,g)\log r+\int_0^r\frac{n(t,g)-n(0,g)}t\,dt,
$$

where $n(0,g)=\max(0,-\nu)$. This convention will also cover $g=f-a$ when the target $a=f(0)$.

Here is a direct proof of the exact reciprocal identity underlying the [Nevanlinna first main theorem](../../../../../nevanlinna-first-main-theorem.md). Choose a circle with no zero or pole of $g$ on it, and a slightly larger disc with the same interior zeros and poles. Divide $g$ by $z^\nu$ and its nonzero zero factors and multiply by its nonzero pole factors, obtaining a [holomorphic](../../../../../complex-differentiability-at-a-point.md), nowhere-zero function $H$ on that disc. For any factor $z-a$ with $|a|<r$,

$$
\frac1{2\pi}\int_0^{2\pi}\log|re^{i\theta}-a|\,d\theta=\log r.
$$

Indeed, factor out $re^{i\theta}$; the remaining logarithm has real part equal to that of $-\sum_{k\ge1}(a/r)^ke^{-ik\theta}/k$, whose angular mean is zero. Also, $\log|H|$ is [harmonic](../../../../../harmonic-function.md), so the [mean value property for harmonic functions](../../../../../mean-value-property-for-harmonic-functions.md) equates its circle mean to $\log|H(0)|$. Putting back the zero and pole factors proves

$$
\frac1{2\pi}\int_0^{2\pi}\log|g(re^{i\theta})|\,d\theta
=\log|c|+N(r,1/g)-N(r,g).
$$

The identity $\log^+x-\log^+(1/x)=\log x$ now yields

$$
\boxed{T(r,g)-T(r,1/g)=\log|c|.}
$$

Zeros or poles on the circle cause only integrable logarithmic singularities; the same identities hold at those radii by limits. A boundary zero or pole contributes $\log(r/r)=0$ to its counting term.

For a finite target $a$, set $g=f-a$. Its finite [poles](../../../../../pole.md) and their orders equal those of $f$. The elementary estimates

$$
\log^+|f-a|\le\log^+|f|+\log(1+|a|),\qquad
\log^+|f|\le\log^+|f-a|+\log(1+|a|)
$$

give $|T(r,f-a)-T(r,f)|\le\log(1+|a|)$. Combining this with the reciprocal identity proves **the first main theorem**:

$$
\boxed{T(r,f)=m(r,1/(f-a))+N(r,1/(f-a))+O(1).}
$$

The error is bounded independently of $r$, with an explicit bound $\log(1+|a|)+|\log|c_a||$, where $c_a$ is the first nonzero local coefficient of $f-a$ at zero. The count on the right records the occurrences of the value $a$ with [multiplicity](../../../../../multiplicity-mathematics.md). The target infinity is the defining identity $T=m+N$. If $f$ is a constant equal to $a$, the reciprocal expression is undefined; the value-distribution assertion assumes $f-a\not\equiv0$, as it automatically does for nonconstant $f$. The exact reciprocal identity remains valid for every nonzero constant $f$.

Taking $g=f$, whose signed order is zero and whose local coefficient is $f(0)$, rearranges that exact identity into [Jensen's formula](../../../../../jensen-s-formula.md):

$$
\boxed{\frac1{2\pi}\int_0^{2\pi}\log|f(re^{i\theta})|\,d\theta
=\log|f(0)|+
\sum_{|z_n|<r}\log\frac r{|z_n|}
-\sum_{|p_n|<r}\log\frac r{|p_n|}.}
$$

Thus the zero and pole terms, their signs and the initial-value constant follow from the same proved identity, rather than from a theorem citation without proof.

Finally let $f$ be a nonzero bounded [holomorphic function](../../../../../holomorphic-function.md) on the [unit disc](../../../../../unit-disc.md), with $|f|\le M$. If its order at zero is $m$, write $f(z)=z^m h(z)$, $h(0)\ne0$. The factorization argument above works on every compact subdisc and gives, for its nonzero zeros,

$$
\sum_{0<|z_n|<r}\log\frac r{|z_n|}
\le\log M-\log|h(0)|-m\log r.
$$

For $1/2\le r<1$ this is a uniform finite upper bound. As $r\uparrow1$, [monotone convergence](../../../../../monotone-convergence-theorem.md) gives

$$
\sum_{z_n\ne0}\log\frac1{|z_n|}<\infty.
$$

Since $1-u\le-\log u$ for $0<u<1$, and there are only $m$ zeros at zero, we obtain

$$
\boxed{\sum_n(1-|z_n|)<\infty.}
$$

This is precisely the [Blaschke condition](../../../../../blaschke-condition.md), so the zeros, counted with [multiplicity](../../../../../multiplicity-mathematics.md), form a [Blaschke sequence](../../../../../blaschke-sequence.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
