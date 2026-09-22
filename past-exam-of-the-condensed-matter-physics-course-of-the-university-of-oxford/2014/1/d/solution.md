<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The FCC parity rule forbids $(100)$ and $(110)$ and allows $(200)$ and $(111)$. To follow each same plane family through the deformation, use fractional coordinates $(x,y,z)$ in the compressed old cell and $(X,Y,Z)$ in the new cube. The preceding vectors give

$$
x=(X-Y)/2,\qquad y=(X+Y)/2,\qquad z=Z.
$$

Thus $hx+ky+lz=m$ becomes $HX+KY+LZ=m$, with

$$
\boxed{(H,K,L)=\left(\frac{h+k}{2},\frac{k-h}{2},l\right).}
$$

Crucially, this transformation retains the plane spacing and diffraction order, not just a normal direction:

| Old FCC reflection | New-cell reciprocal coordinates | Status |
| --- | --- | --- |
| $(100)$ | $(\tfrac12,-\tfrac12,0)$ | Not a new reciprocal-lattice vector; absent |
| $(110)$ | $(1,0,0)$ | Odd index sum; absent |
| $(200)$ | $(1,-1,0)$ | Even index sum; allowed |
| $(111)$ | $(1,0,1)$ | Even index sum; allowed |

The two physically allowed reflections remain allowed, and the two absent ones remain absent. Their angles and spacings change under strain; their allowedness as tracked reciprocal vectors does not.

The half-integer entry is deliberate. It cannot be relabeled as the ordinary BCC $(1\bar10)$ reflection while claiming to track the same diffraction order. Multiplying its indices by two doubles the reciprocal vector and halves the spacing; that new allowed reflection is the image of old FCC $(200)$, not old $(100)$. If only an orientation label is wanted, the old $(100)$ and $(200)$ planes both have the new $(1\bar10)$ orientation, but are distinct orders. This is the distinction between [diffraction indexing under a cell change](../../../../diffraction-indexing-under-a-cell-change.md) and merely reducing a plane normal to the smallest integer ratio.

## ↑ Ancestors (12)

1. [D](../d.md)
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
