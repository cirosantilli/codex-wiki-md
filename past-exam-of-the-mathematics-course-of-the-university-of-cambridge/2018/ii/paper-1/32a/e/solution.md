<h1 id="32a/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The Hamiltonian in the question is

$$
H=\frac12\bar z_jz_j
=\frac12\sum_{j=1}^n(q_j^2+p_j^2).
$$

Define

$$
I_j=\frac12|z_j|^2=\frac12(q_j^2+p_j^2).
$$

Each $I_j$ is a first integral, the functions involve disjoint canonical coordinate pairs and hence satisfy $\{I_j,I_k\}=0$, and their differentials are independent wherever every $z_j\ne0$. Since $H=\sum_jI_j$, these $n$ integrals prove [Liouville integrability of the isotropic harmonic oscillator](../../../../../../liouville-integrability-of-the-isotropic-harmonic-oscillator.md).

For constants $c_j>0$, the common level is

$$
I_j=c_j
\quad\Longleftrightarrow\quad
|z_j|=\sqrt{2c_j},
$$

so the regular invariant set is

$$
\boxed{\ S^1_{\sqrt{2c_1}}\times\cdots\times S^1_{\sqrt{2c_n}}\cong\mathbb T^n.\ }
$$

Hamilton's equations give $\dot z_j=-iz_j$, so every angle evolves as $\theta_j(t)=\theta_j(0)-t$. If some $c_j=0$, the corresponding circle collapses and the level is a lower-dimensional singular invariant torus.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [32A](../../32a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
