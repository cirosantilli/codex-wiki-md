<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $q_j$ denote the four critical [wavevectors](../../../../../../wavevector.md), and write $A_j=R_je^{i\theta_j}$. A spatial translation by $(s,t)$ acts on the [amplitudes](../../../../../../wave-amplitude.md) as

$$
(A_1,A_2,A_3,A_4)\longmapsto
(e^{i(2s+t)}A_1,e^{i(2s-t)}A_2,e^{i(s+2t)}A_3,e^{i(s-2t)}A_4).
$$

The two independent translation directions in [phase space](../../../../../../phase-space.md) are $(2,2,1,1)$ and $(1,-1,2,-2)$. Their common orthogonal complement is spanned by $(2,-2,-1,1)$ and $(1,1,-2,-2)$. Hence [translation invariants of Fourier-mode phases](../../../../../../translation-invariants-of-fourier-mode-phases.md) can be chosen as

$$
\boxed{\chi_1=2\theta_1-2\theta_2-\theta_3+\theta_4,\qquad
\chi_2=\theta_1+\theta_2-2\theta_3-2\theta_4.}
$$

Away from zero [amplitudes](../../../../../../wave-amplitude.md), a translation-invariant function of the [phases](../../../../../../phase-waves.md) is a function of these two invariant angles. The four magnitudes are themselves invariant. Thus an [equivariant dynamical system](../../../../../../equivariant-dynamical-system.md) on the eight-real-dimensional [centre manifold](../../../../../../center-manifold.md) descends, after quotienting [translation symmetry](../../../../../../translational-symmetry.md), to **four magnitude equations and two invariant-phase equations**. The [phase](../../../../../../phase-waves.md) coordinates are singular where an [amplitude](../../../../../../wave-amplitude.md) vanishes; the original complex-amplitude equations remain smooth there.

The [wavevector selection rule for equivariant monomials](../../../../../../wavevector-selection-rule-for-equivariant-monomials.md) proves the cubic regularity. For a [monomial](../../../../../../monomial.md) $\prod_jA_j^{p_j}\overline A_j^{q_j}$ in the first equation, put $d_j=p_j-q_j$. Translation covariance requires

$$
2d_1+2d_2+d_3+d_4=2,\qquad d_1-d_2+2d_3-2d_4=1.
$$

At total degree $N$, additionally $\sum|d_j|\leq N$ and $N-\sum|d_j|$ is even. Conversely, any integer vector satisfying these conditions yields a [monomial](../../../../../../monomial.md), with any remaining even degree supplied by factors $|A_j|^2$. This makes the degree test exhaustive. For example, eliminate the first two entries:

$$
d_1=\frac{4-5d_3+3d_4}{4},\qquad
d_2=\frac{3d_3-5d_4}{4}.
$$

Checking the integer pairs $|d_3|+|d_4|\leq N$, retaining only integral $d_1,d_2$ with the norm and parity conditions, gives

$$
\begin{array}{c|c}
N&\text{admissible }d\\\hline
1&(1,0,0,0)\\
3&(1,0,0,0)\\
5&(1,0,0,0),\ (-1,2,1,-1),\ (0,-1,2,2).
\end{array}
$$

At degree three the only possibility is therefore $A_1|A_j|^2$, $j=1,\ldots,4$. Square [symmetry](../../../../../../symmetry-physics.md) gives the same conclusion for every other equation. All cubic terms are regular.

Two generators of the square [dihedral group](../../../../../../dihedral-group.md) act as follows. [Reflection](../../../../../../reflection-mathematics.md) in the $x$ axis gives $(A_1,A_2,A_3,A_4)\mapsto(A_2,A_1,A_4,A_3)$, while interchange of $x,y$ gives $(A_3,\overline A_4,A_1,\overline A_2)$. Rotation by $\pi$ conjugates every [amplitude](../../../../../../wave-amplitude.md), forcing the [coefficients](../../../../../../coefficient.md) in a steady [normal form of a dynamical system](../../../../../../normal-form-dynamical-systems.md) to be real. With real unfolding parameter $\sigma$ and real [coefficients](../../../../../../coefficient.md) $c_1,c_2,c_3,c_4$, define

$$
\begin{aligned}
G_1&=\sigma+c_1|A_1|^2+c_2|A_2|^2+c_3|A_3|^2+c_4|A_4|^2,\\
G_2&=\sigma+c_1|A_2|^2+c_2|A_1|^2+c_3|A_4|^2+c_4|A_3|^2,\\
G_3&=\sigma+c_1|A_3|^2+c_2|A_4|^2+c_3|A_1|^2+c_4|A_2|^2,\\
G_4&=\sigma+c_1|A_4|^2+c_2|A_3|^2+c_3|A_2|^2+c_4|A_1|^2.
\end{aligned}
$$

The **most general cubic normal form is $\dot A_j=A_jG_j+O(|A|^5)$**. There are no further [coefficient](../../../../../../coefficient.md) identifications: the square-group stabilizer of one of these oblique [wavevectors](../../../../../../wavevector.md) is trivial, so its three couplings to the other magnitudes are independent. At cubic order $\dot R_j=R_jG_j$ and all [phases](../../../../../../phase-waves.md), including $\chi_1,\chi_2$, are constant.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
