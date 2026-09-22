<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Put $S(\theta)=\sum_{r=1}^n e(\theta r^3)$. Its modulus is the modulus of the [Fourier transform](../../../../../fourier-transform.md) in the question, independently of the sign convention. We use [Hua's lemma](../../../../../hua-s-lemma.md) in the cubic form $\int_0^1|S|^8\ll_\delta n^{5+\delta}$; the [cubic eighth-moment proof by differencing](../../../../../cubic-eighth-moment-proof-by-differencing.md) establishes this from the [subpower bound for the divisor function](../../../../../subpower-bound-for-the-divisor-function.md). Therefore

$$
\frac{N^2}{2007}\le\int_m|S|^9\le\sup_{\theta\in m}|S(\theta)|\int_0^1|S|^8
$$

and $n\asymp N^{1/3}$ imply $\sup_m|S|\gg_\delta n^{1-\delta}$. Choose an actual $\theta\in m$ attaining at least half this bound; attainment of the supremum itself is unnecessary.

Fix $\varepsilon>0$ and put $\varepsilon_0=\min(\varepsilon,1/6)$. The [Dirichlet approximation theorem](../../../../../dirichlet-s-approximation-theorem.md) with $Q=\lfloor N^{1-\varepsilon_0}\rfloor$ gives [coprime integers](../../../../../coprime-integers.md) $a,q$ satisfying

$$
1\le q\le Q,\qquad \|q\theta\|\le Q^{-1},\qquad |\theta-a/q|\le(qQ)^{-1}\le q^{-2}.
$$

The [cubic Weyl inequality](../../../../../cubic-weyl-inequality.md), which is the quantitative equidistribution estimate needed here, says

$$
|S(\theta)|\ll_\eta n^{1+\eta}\left(q^{-1}+n^{-1}+q/n^3\right)^{1/4}.
$$

Compare it with the lower bound. Choose $\delta,\eta>0$ so small that $b=4(\delta+\eta)/3<\varepsilon_0/2$. It follows that

$$
q^{-1}+n^{-1}+q/n^3\gg_{\delta,\eta}N^{-b}.
$$

But $n^{-1}=O(N^{-1/3})$ and $q/n^3=O(N^{-\varepsilon_0})$. Both are $o(N^{-b})$, so for large $N$ the first term must supply this lower bound. Consequently $q\ll_\varepsilon N^b\ll_\varepsilon N^\varepsilon$, while the approximation above gives $\|q\theta\|\ll N^{\varepsilon_0-1}\le N^{\varepsilon-1}$. Enlarging the constants covers bounded $N$. Thus

$$
\boxed{\theta\in m,\qquad q\ll_\varepsilon N^\varepsilon,\qquad \|q\theta\|\ll_\varepsilon N^{\varepsilon-1}.}
$$

Here $\|\cdot\|$ is [distance modulo one](../../../../../distance-to-the-nearest-integer.md). A ninth moment of this size therefore forces at least one near-rational frequency, rather than merely a large pointwise sum somewhere outside $m$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
