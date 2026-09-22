<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use zero-based indices $0\leq i<2^n$; the two index conventions in the printed question enumerate the same partition. Let $O_n(\gamma)$ be the sum of length powers over odd intervals and $H_n(\gamma)$ the sum over all intervals. For odd-address words, the given [symbolic potential](../../../../../../symbolic-potential.md) estimate has $c\leq|\Delta_i^{(n)}|e^{-H_n^{\rm pot}(i)}\leq C$, with constants independent of $n,i$. Raising these bounds to a fixed real power $\gamma$ and reversing the order when necessary gives finite positive constants $c_\gamma,C_\gamma$ such that

$$
c_\gamma Z_n(\gamma)\leq O_n(\gamma)\leq C_\gamma Z_n(\gamma).
$$

Therefore $n^{-1}\log O_n(\gamma)\to f(\gamma)$. It remains to justify the even intervals, since the supplied estimate covers only half of the partition.

In the standard period-doubling partition, $\Delta_0^{(n)}=\beta^n[-1,1]$ and $\Delta_i^{(n)}=g^i(\Delta_0^{(n)})$. All odd-address intervals lie in the first image restrictive interval, a compact set away from the unique critical point zero. Hence there are uniform constants $0<d\leq|g'|\leq D_1$ there. For an odd $i<2^n-1$, its image is the next even interval, and the [mean value theorem](../../../../../../mean-value-theorem.md) gives $d|\Delta_i^{(n)}|\leq|\Delta_{i+1}^{(n)}|\leq D_1|\Delta_i^{(n)}|$.

For the wraparound pair the image of the last interval is a subinterval of $\Delta_0^{(n)}$, not necessarily the whole of it. Iterating the renormalization identity gives

$$
g^{2^n}(\beta^nx)=\beta^ng(x).
$$

Thus $|g(\Delta_{2^n-1}^{(n)})|=|\beta|^n(1-\beta)$, while $|\Delta_0^{(n)}|=2|\beta|^n$. The image is the fixed fraction $(1-\beta)/2$ of the central interval. Combining this with the derivative bounds proves uniform comparability of the last odd interval and the central even interval as well. This establishes the [odd-even comparison for Feigenbaum partition lengths](../../../../../../odd-even-comparison-for-feigenbaum-partition-lengths.md) for every pair, including wraparound.

Consequently, for each fixed real $\gamma$, the even sum is bounded above and below by constant multiples of $O_n(\gamma)$. The same is true of $H_n(\gamma)$, so

$$
\boxed{f(\gamma)=\lim_{n\to\infty}\frac1n\log\sum_{i=0}^{2^n-1}|\Delta_i^{(n)}|^\gamma.}
$$

Finally take $\gamma>\gamma_*$. Strict decrease gives $f(\gamma)<0$, so this length-power sum tends to zero exponentially. The cover mesh also tends to zero: negative bounded $U$ and the odd-interval estimate give $|\Delta_i^{(n)}|\leq Ce^{-bn}$ on odd intervals, and the odd-even comparison transfers this bound to all intervals. Since the intervals cover the [Feigenbaum attractor](../../../../../../feigenbaum-attractor.md), they are admissible arbitrarily fine covers in the definition of [Hausdorff measure](../../../../../../hausdorff-measure.md), and $\mathcal H^\gamma(F)=0$. Therefore the [pressure upper bound for Hausdorff dimension](../../../../../../pressure-upper-bound-for-hausdorff-dimension.md) yields

$$
\boxed{\dim_H F\leq\gamma_* .}
$$

The covering argument supplies the requested upper bound; it does not assume a dimension equality or a lower bound not proved here.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
