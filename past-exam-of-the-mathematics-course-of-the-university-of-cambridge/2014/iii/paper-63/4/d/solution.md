<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $\lambda=2ks$. For $t\geq0$, apply a valid [Lieb-Robinson bound](../../../../../../lieb-robinson-bound.md) to each [commutator](../../../../../../commutator.md) in the supplied comparison of the two evolutions. For a disjoint shell at support distance $d$,

$$
\|[h_Z(\tau),h_Y]\|\leq2\|h_Z\|\|h_Y\|\min(|Z|,|Y|)e^{-\mu d}(e^{\lambda\tau}-1).
$$

In the usual uniform interaction-norm setting, truncation preserves the strength bound, so the same constants apply to $H_d$. The given polynomial shell-weight hypothesis and $e^{\lambda\tau}-1\leq e^{\lambda t}$ now give

$$
\begin{aligned}
\|e^{itH_d}h_Ze^{-itH_d}-e^{itH_{d-1}}h_Ze^{-itH_{d-1}}\|&\leq C\|h_Z\|d^\alpha e^{-\mu d}\int_0^te^{\lambda\tau}d\tau\\
&\leq C\|h_Z\|t d^\alpha e^{-\mu d+\lambda t}.
\end{aligned}
$$

Consequently

$$
\boxed{\|e^{itH_d}h_Ze^{-itH_d}-e^{itH_{d-1}}h_Ze^{-itH_{d-1}}\|=O(\|h_Z\|\,|t|d^\alpha e^{-\mu d+2ks|t|}).}
$$

The question explicitly supplies a bound for the full $H$; such a bound alone should not be assumed to transfer to $H_d$. A [full-evolution comparison for truncated dynamics](../../../../../../full-evolution-comparison-for-truncated-dynamics.md) avoids that additional assumption. The Duhamel comparison formula gives

$$
\|\tau_t^H(h_Z)-\tau_t^{H_j}(h_Z)\|\leq\sum_{Y:d(Z,Y)>j}\int_0^{|t|}\|[\tau_\sigma^H(h_Z),h_Y]\|d\sigma.
$$

Now use only the full-Hamiltonian bound, and sum the shell weights. Since $\sum_{q\geq d}q^\alpha e^{-\mu q}=O(d^\alpha e^{-\mu d})$, the errors for $j=d$ and $j=d-1$ are each bounded by $O(\|h_Z\||t|d^\alpha e^{-\mu d+\lambda|t|})$. The triangle inequality comparing both evolutions to $\tau_t^H(h_Z)$ proves the same boxed estimate from the stated full-system assumption. Negative times follow by the reverse-time Duhamel formula; the [commutator](../../../../../../commutator.md) bounds use $|t|$.

For the interaction-term shells used to enforce $H_0=h_Z$, shell $d$ corresponds to support distance $d-1$ for distinct terms. Replace the displayed [commutator](../../../../../../commutator.md) estimate by the coarser bound with $e^{\lambda\tau}$, retaining the equal-time contribution for overlaps. Its distance factor is $e^{-\mu(d-1)}=e^\mu e^{-\mu d}$, and the fixed factor $e^\mu$ is absorbed by the big-O constant. This supplies the same claimed shell estimate without incorrectly using a zero equal-time bound for overlapping terms.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
