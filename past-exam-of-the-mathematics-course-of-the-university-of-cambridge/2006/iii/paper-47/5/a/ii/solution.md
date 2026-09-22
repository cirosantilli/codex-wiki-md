<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An [independence sampler](../../../../../../../independence-metropolis-hastings-algorithm.md) proposes from a fixed density $g(\theta')$, independent of the current state. Its acceptance probability is

$$
\boxed{\alpha(\theta,\theta')=\min\left\{1,
\frac{\pi(\theta')g(\theta)}{\pi(\theta)g(\theta')}\right\}.}
$$

If $g$ is close to the target, proposals can make large efficient moves and cross separated modes; $g=\pi$ gives acceptance one and independent samples. On the other hand, a good global approximation is required. A proposal with tails too light can leave the chain trapped at states having very large importance weight $\pi/g$, since most outgoing proposals then have tiny acceptance probabilities.

For perspective, if the normalized target satisfies $\pi\le Mg$, the accepted transition density is at least $\pi(\theta')/M$, because both entries in $\min\{g(\theta'),\pi(\theta')/w(\theta)\}$ have that lower bound, where $w=\pi/g\le M$. This yields a uniform refresh component. Thus a well-designed independence proposal can mix rapidly, whereas a poor global proposal can be much worse than a locally tuned random walk. The tradeoff concerns effective samples per computation, not acceptance rate alone.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
