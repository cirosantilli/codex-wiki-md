<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

We first prove that every extension of two simple modules splits. Consider

$$
0\longrightarrow A_n\longrightarrow V\longrightarrow A_m\longrightarrow0.
$$

If $n\ne m$, the central [Casimir element](../../../../casimir-element.md) has distinct scalars $n(n+2)$ and $m(m+2)$. On $V$ its [minimal polynomial](../../../../minimal-polynomial.md) divides the product of the corresponding two distinct linear factors. Its eigenspaces are submodules, and the [eigenspace](../../../../eigenspace.md) for $m(m+2)$ maps isomorphically onto the [quotient](../../../../quotient.md). It is the required complement.

Now suppose $n=m=l$. Use [generalized weight spaces](../../../../generalized-weight-space-of-a-lie-algebra-representation.md) for $H$; their possible weights are $l,l-2,\ldots,-l$, because the [characteristic polynomial](../../../../characteristic-polynomial.md) on an extension is the product of those on its two factors. Lift the [quotient](../../../../quotient.md)'s highest vector to $w$ in the [generalized weight space](../../../../generalized-weight-space-of-a-lie-algebra-representation.md) of [representation weight](../../../../weight-of-a-representation.md) $l$. Then $ew=0$ and $f^{l+1}w=0$, since these would lie in [generalized weight spaces](../../../../generalized-weight-space-of-a-lie-algebra-representation.md) of weights $l+2$ and $-l-2$, which are absent. Also $(H-l)w=av_0$ for a highest vector $v_0$ in the [submodule](../../../../submodule.md) $A_l$. The commutator identity gives

$$
0=ef^{l+1}w=(l+1)f^l(H-l)w=(l+1)a f^lv_0.
$$

Thus $a=0$. The vector $w$ is an actual highest-[weight vector](../../../../weight-vector.md). Its lowering chain maps to the full [basis](../../../../basis.md) of the [quotient](../../../../quotient.md), so it generates an $A_l$ complementary to the original [submodule](../../../../submodule.md). This proves splitting also when the two simple types coincide, including $l=0$.

The same splitting holds for a semisimple [kernel](../../../../kernel-of-a-linear-map-split.md) and simple [quotient](../../../../quotient.md) by induction on the number of [kernel](../../../../kernel-of-a-linear-map-split.md) summands. Write the [kernel](../../../../kernel-of-a-linear-map-split.md) as $U_1\oplus U_2$ with $U_1$ simple. Modulo $U_2$, split the extension by the simple [quotient](../../../../quotient.md); the inverse image of that chosen [quotient](../../../../quotient.md) copy is an extension with [kernel](../../../../kernel-of-a-linear-map-split.md) $U_2$. Split it inductively, obtaining a [submodule](../../../../submodule.md) in $V$ meeting the entire original [kernel](../../../../kernel-of-a-linear-map-split.md) trivially.

Finally induct on $\dim V$. A maximal proper [submodule](../../../../submodule.md) has smaller [dimension](../../../../dimension-vector-space.md) and hence is semisimple by induction; the [quotient](../../../../quotient.md) is simple by maximality. The just-proved splitting completes the induction. Hence

$$
\boxed{V\cong\bigoplus_{l\ge0}A_l^{\oplus m_l},\qquad m_l\in\mathbb Z_{\ge0},}
$$

with only finitely many nonzero multiplicities. This proof does not assume the complete-reducibility theorem it is establishing.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the representation theory of semisimple Lie algebras course of the University of Oxford](../../../split.md)
5. [Representation theory of semisimple Lie algebras course of the University of Oxford](../../../../representation-theory-of-semisimple-lie-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
