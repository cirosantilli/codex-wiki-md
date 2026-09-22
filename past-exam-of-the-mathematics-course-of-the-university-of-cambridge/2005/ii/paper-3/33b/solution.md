<h1 id="33b/solution">Solution</h1>

↑ **Parent:** [33B](../33b.md)

A [Bravais lattice](../../../../../bravais-lattice.md) is the set of all integer combinations of linearly independent primitive translation vectors. Its [reciprocal lattice](../../../../../reciprocal-lattice.md) consists of $g$ satisfying $g\cdot l\in2\pi\mathbb Z$ for every translation $l$; equivalently $e^{ig\cdot l}=1$.

The original PDF's third family has a bare $j$, not $n_2j$. Taken literally, the listed set is not the claimed [Bravais lattice](../../../../../bravais-lattice.md): the claimed primitive vector $a(i+k)/2$ does not occur. Its half-integer first and third coordinates force it into that third family, whose second coordinate is always $a$, not zero. The intended repair is **$j\mapsto n_2j$ in the third family**. The following conclusions apply to that corrected set.

The four corrected families are exactly

$$
L=\frac a2\{(h,k,l)\in\mathbb Z^3:h+k+l\text{ is even}\}.
$$

The allowed parity patterns are all even, or exactly two odd coordinates. An integer combination of the proposed primitive vectors has coordinates $(a/2)(m_2+m_3,m_1+m_3,m_1+m_2)$, so lies in this set. Conversely, solve

$$
m_1=\tfrac12(k+l-h),\quad m_2=\tfrac12(h+l-k),\quad m_3=\tfrac12(h+k-l).
$$

All three are integers precisely when $h+k+l$ is even. This proves that the corrected set is the [face-centered cubic lattice](../../../../../face-centered-cubic-lattice.md) with the proposed primitive basis.

Direct dot products give $a_i\cdot b_j=2\pi\delta_{ij}$ for

$$
\boxed{b_1=\frac{2\pi}a(-1,1,1),\quad b_2=\frac{2\pi}a(1,-1,1),\quad b_3=\frac{2\pi}a(1,1,-1).}
$$

These vectors generate the entire [reciprocal lattice](../../../../../reciprocal-lattice.md), since the coefficients of an arbitrary reciprocal vector in this basis are its integer pairings with the $a_i$. Its vectors are $(2\pi/a)(h,k,l)$ with all three coordinates of the same parity, the [body-centered cubic lattice](../../../../../body-centered-cubic-lattice.md).

In [Bragg scattering](../../../../../bragg-scattering.md), translating a scattering atom by $l$ changes the amplitude by $e^{i(k-k')\cdot l}$. Constructive interference from every lattice translate requires this factor to be one, so $k'-k=g$ is a [reciprocal lattice](../../../../../reciprocal-lattice.md) vector. For elastic scattering, $|k'|=|k|$; the chord between these two vectors has length $2|k|\sin(\theta/2)$. Therefore

$$
\boxed{\sin(\theta/2)=\frac{|g|}{2|k|}.}
$$

The shortest nonzero reciprocal vectors are the $(111)$ family of length $(2\pi/a)\sqrt3$, followed by the $(200)$ family of length $(2\pi/a)2$. Identical atoms on this [Bravais lattice](../../../../../bravais-lattice.md) introduce no additional basis extinction. If both families are accessible at the incident wavelength, their scattering angles obey **$\boxed{\sin(\theta_1/2)/\sin(\theta_2/2)=\sqrt3/2}$**.

## ↑ Ancestors (10)

1. [33B](../33b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
