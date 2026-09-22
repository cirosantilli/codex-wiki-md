<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use fractional coordinates relative to conventional cubic vectors $(a\hat x,a\hat y,a\hat z)$. A [body-centered cubic lattice](../../../../body-centered-cubic-lattice.md) has representative points

$$
(0,0,0),\quad(\tfrac12,\tfrac12,\tfrac12),
$$

so its conventional cell contains two [lattice points](../../../../lattice-point.md): eight shared corners contribute one and the interior point contributes one. A [face-centered cubic lattice](../../../../face-centered-cubic-lattice.md) has

$$
(0,0,0),\quad(0,\tfrac12,\tfrac12),\quad(\tfrac12,0,\tfrac12),\quad(\tfrac12,\tfrac12,0),
$$

so its conventional cell contains four: one from the shared corners and three from six half-shared faces.

For $N$ atoms at fractional positions $(x_j,y_j,z_j)$, the geometric [structure factor](../../../../structure-factor.md) and the atomic-factor-weighted amplitude are respectively

$$
G_{hkl}=\sum_{j=1}^N e^{2\pi i(hx_j+ky_j+lz_j)},\qquad
F_{hkl}=\sum_{j=1}^N f_j(\mathbf G)e^{2\pi i(hx_j+ky_j+lz_j)}.
$$

For identical atoms $F=fG$. Applying the conventional-cell lattice factors gives

$$
\boxed{G_{\rm BCC}=1+(-1)^{h+k+l}=\begin{cases}2,&h+k+l\text{ even},\\0,&h+k+l\text{ odd},\end{cases}}
$$

and

$$
\boxed{G_{\rm FCC}=1+(-1)^{k+l}+(-1)^{h+l}+(-1)^{h+k}
=\begin{cases}4,&h,k,l\text{ all even or all odd},\\0,&\text{mixed parity}.\end{cases}}
$$

These are lattice selection rules; an additional nontrivial [crystal basis structure factor](../../../../crystal-basis-structure-factor.md) can extinguish further allowed reflections.

Of the eight equally represented parity triples, four satisfy the BCC condition and two the FCC condition. Thus the fractions among integer index triples are $1/2$ and $1/4$, respectively. This reflects the two and four equivalent [lattice points](../../../../lattice-point.md) in the conventional cells: their reciprocal lattices occupy corresponding subsets of the conventional reciprocal grids. In primitive reciprocal coordinates every integer triple denotes a reciprocal-lattice vector; lattice-centering absences are then built into the grid rather than an extra rule. A multi-atom chemical basis can still cause genuine additional absences. If permutations means merely reordering one fixed triple, its allowedness never changes: the quoted fractions concern all index triples, not reordering a chosen $(h,k,l)$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
