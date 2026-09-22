<h1 id="12/solution">Solution</h1>

↑ **Parent:** [12](../12.md)

**The [Pusey-Barrett-Rudolph theorem](../../../pusey-barrett-rudolph-theorem.md) excludes overlapping preparation distributions for distinct [pure states](../../../pure-state.md) in an [ontological model of a quantum system](../../../ontological-model-of-a-quantum-system.md) satisfying [preparation independence](../../../preparation-independence.md) and the specified quantum predictions. It excludes neither all hidden variables nor every informational use of a [quantum state](../../../quantum-state.md).** The precise overlap criterion is essential: a [psi-epistemic model](../../../psi-epistemic-model.md) lets at least two distinct pure-state preparations assign positive common probability mass to the same underlying states; a [psi-ontic model](../../../psi-ontic-model.md) has mutually singular measures for each distinct pair.[classification of ontological models and the distinction between epistemic overlap and ontic incompleteness](../../../einstein-incompleteness-and-the-epistemic-view-of-quantum-states-by-nicholas-harrigan-and-robert-w-spekkens.md)

Let preparation $x$ sample $\lambda\in\Lambda$ from $\mu_x$. A fixed [quantum measurement](../../../quantum-measurement-split.md) $M$ has nonnegative response functions $\xi_M(j|\lambda)$ with $\sum_j\xi_M(j|\lambda)=1$. Averaging over the preparation must reproduce the [Born rule](../../../born-rule.md). The response is fixed by $M$ and the complete underlying state, not by additional knowledge of the preparation label. No [outcome determinism](../../../outcome-determinism.md) or [Bell local causality](../../../bell-local-causality.md) is assumed; the joint measurement response need not factor into local responses. For independently operated preparations, [preparation independence](../../../preparation-independence.md) further identifies the joint state space with the appropriate product and assigns

$$
\mu_{x_1\ldots x_n}(\lambda_1,\ldots,\lambda_n)
=\prod_{k=1}^n\mu_{x_k}(\lambda_k).
$$

Operationally independent devices do not logically entail this ontic factorization; it is an additional physical premise.[arXiv:1111.3328v3, pp. 2–4, equations (1)–(5): preparation measures, independent composition and normalized measurement response](../../../on-the-reality-of-the-quantum-state-by-matthew-f-pusey-and-others.md)

The two-[qubit](../../../qubit.md) example can be checked directly. Set $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$. In [computational basis](../../../computational-basis.md) order $00,01,10,11$, take the following normalized columns as an [orthonormal basis](../../../orthonormal-basis.md):

$$
\xi_1=\frac{(0,1,1,0)^T}{\sqrt2},\quad
\xi_2=\frac{(1,-1,1,1)^T}{2},\quad
\xi_3=\frac{(1,1,-1,1)^T}{2},\quad
\xi_4=\frac{(1,0,0,-1)^T}{\sqrt2}.
$$

Their pairwise [inner products](../../../inner-product-split.md) vanish. Direct multiplication shows that the respective preparations $00,0+,+0,++$ have zero [probability amplitude](../../../probability-amplitude.md) for respective outcomes $1,2,3,4$. This is the [PBR exclusion measurement for zero and plus](../../../pbr-exclusion-measurement-for-zero-and-plus.md): the measurement does not perfectly distinguish the preparations, but each outcome rules one out.

Suppose a common submeasure $\nu$ of $\mu_0$ and $\mu_+$ has mass $\omega>0$; with densities one can take $\nu(\lambda)=\min\{\mu_0(\lambda),\mu_+(\lambda)\}$. [Preparation independence](../../../preparation-independence.md) makes $\nu\otimes\nu$ a common submeasure of all four product preparations, of mass $\omega^2$. The zero probability for outcome $j$ under its excluded preparation and nonnegativity force

$$
\int\xi_M(j|\lambda_1,\lambda_2)\,d(\nu\otimes\nu)=0
\quad(j=1,2,3,4).
$$

Summing and using normalization yields $\omega^2=0$, a contradiction. This measure formulation avoids treating a set with merely nonempty topological support as a positive-probability overlap.

For arbitrary distinct nonorthogonal [pure states](../../../pure-state.md), write $|\psi_{0,1}\rangle=\cos(\theta/2)|0\rangle\pm\sin(\theta/2)|1\rangle$, with overlap $\cos\theta$ and $0<\theta<\pi/2$. The general proof constructs an exclusion measurement on $n$ independently prepared copies when $2^{1/n}-1\leq\tan(\theta/2)$. A finite $n$ always exists. The same common-submeasure contradiction then excludes positive overlap. Orthogonal preparations are already disjoint if their perfectly distinguishing measurement is reproduced. The original paper also bounds residual overlap for imperfect exclusion data; exact disjointness concerns the ideal theorem, not a finite experiment's proof of exact zero.[pp. 3–4 and Appendices A–B: finite-copy condition and noise-robust bound](../../../on-the-reality-of-the-quantum-state-by-matthew-f-pusey-and-others.md)

The scope is consequently sharp. [Bohmian mechanics](../../../de-broglie-bohm-theory.md) is not excluded: its underlying state includes the [wave function](../../../wave-function-split.md), making distinct pure preparations disjoint even though extra configuration variables remain. A [psi-ontic model](../../../psi-ontic-model.md) need not be complete with the [wave function](../../../wave-function-split.md) alone, and the theorem does not identify the [wave function](../../../wave-function-split.md) with a three-dimensional material [field](../../../field.md). Models abandoning [preparation independence](../../../preparation-independence.md), or accounts not representing preparations as uncertainty over observer-independent states of this specified kind, are outside this conclusion. Epistemic uncertainty between mixed preparations is not banned. Nor does the theorem establish a collapse mechanism, choose between Bohmian and Everettian theories, or solve the [measurement problem](../../../measurement-problem.md). Its achievement is a conditional impossibility theorem about a precise form of pure-state epistemic overlap.

## ↑ Ancestors (10)

1. [12](../12.md)
2. [2019](../../2019-split.md)
3. [Past exam of the philosophy of space-time and philosophy of quantum mechanics paper of Parts A and B of the physics course of the University of Oxford](../../split.md)
4. [Philosophy of space-time and philosophy of quantum mechanics paper of Parts A and B of the physics course of the University of Oxford](../../../philosophy-of-space-time-and-philosophy-of-quantum-mechanics-paper-of-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
5. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
6. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
