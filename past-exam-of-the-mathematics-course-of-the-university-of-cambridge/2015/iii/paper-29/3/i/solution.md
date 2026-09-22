<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First prove [nowhere monotonicity of Brownian motion](../../../../../../nowhere-monotonicity-of-brownian-motion.md). On a fixed interval $[a,b]$ with rational endpoints and $a<b$, the $2^m$ increments over its equal subdivision are independent centered [normal random variables](../../../../../../gaussian-random-variable.md). If the [Brownian motion](../../../../../../brownian-motion-split.md) path were nondecreasing, all these increments would be nonnegative, an event with probability $2^{-2^m}$. Letting $m\to\infty$ gives probability zero. The same argument excludes nonincreasing paths. A countable union over rational intervals shows that, [almost surely](../../../../../../almost-sure-convergence.md), no nontrivial interval supports a [monotone function](../../../../../../monotonic-function.md) restriction of the path, since every such interval contains one with rational endpoints.

Work on this event and on the event of continuous paths. Inside any open interval $I\subset(0,\infty)$, choose two separated smaller intervals, the first to the left of the second. The first contains $r<s$ with $B_r<B_s$, because its restriction is not nonincreasing. The second contains $u<v$ with $B_u>B_v$, because its restriction is not nondecreasing. Thus $r<s<u<v$, all in $I$.

By the [extreme value theorem](../../../../../../extreme-value-theorem.md), the path attains its maximum on $[r,v]$. This value exceeds $B_r$, since it is at least $B_s$, and exceeds $B_v$, since it is at least $B_u$. A maximizing time therefore lies in $(r,v)$ and is a [local maximum of Brownian motion](../../../../../../local-maximum-of-brownian-motion.md). Every open interval in the half-line contains a positive-time interval of this kind. Consequently **the set of [local maxima of Brownian motion](../../../../../../local-maximum-of-brownian-motion.md) is dense in $[0,\infty)$ [almost surely](../../../../../../almost-sure-convergence.md)**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
