<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a short inducer pulse to release [DNA](../../../../deoxyribonucleic-acid.md)-bound fluorescent [LacI](../../../../laci.md), then remove extracellular [IPTG](../../../../isopropyl-beta-d-1-thiogalactopyranoside.md) rapidly and start the search clock after washout. The supplied entry, binding and dissociation times imply a synchronization uncertainty of order a few tenths of a second, which must be measured and separated from the search latency. If rebinding is faster than that dead time, the protocol alone cannot resolve the true mean without a kinetic correction or faster triggering.

Image individual cells rapidly enough to distinguish freely diffusing [proteins](../../../../protein-split.md) from a persistent immobilized fluorescent spot at the single operator. Prelocate that locus from an independent position marker or a previous binding event. Score the first specific capture after each reset; controls lacking a functional target distinguish stable operator binding from nonspecific [DNA](../../../../deoxyribonucleic-acid.md) residence. Correct for localization error, [bleaching](../../../../photobleaching.md), blinking, missed brief events and target motion, and verify that the fluorescent tag does not substantially change the search kinetics.

With four independent freely searching [molecules](../../../../molecule-split.md), each having an approximately exponential single-[molecule](../../../../molecule-split.md) target-arrival time of mean $\tau_1$, the first-arrival survival is

$$
S(t)=e^{-4t/\tau_1},\qquad\boxed{\tau_1=4\langle t_{\rm first}\rangle.}
$$

Thus report both the observed first capture among four and the inferred mean for one searcher. If the number of visible available [molecules](../../../../molecule-split.md) varies, use $S(t)=\exp[-\int_0^t n(s)ds/\tau_1]$ and account for censoring rather than blindly multiplying by four. Repeated resets and many cells estimate the distribution; deviations from an exponential test the independent well-mixed approximation. The rapid inducer manipulation defines a synchronization strategy, not an assumption that all subsequent intracellular search paths are identical.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
