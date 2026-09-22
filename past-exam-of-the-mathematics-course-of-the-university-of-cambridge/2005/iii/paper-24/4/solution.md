<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $Z=\mathbb{CP}^5/\mathbb{CP}^2$. Its quotient cell structure has one cell in each of dimensions $0,6,8,10$. In particular $Z$ is five-connected. The relative [cohomology](../../../../../cohomology-split.md) sequence, or its [cellular cochain complex](../../../../../cellular-cochain-complex.md), gives

$$
H^*(Z;\mathbb Q)=\mathbb Q\oplus\mathbb Qa_6\oplus\mathbb Qb_8\oplus\mathbb Qc_{10}.
$$

The subscripts denote degrees. Under the quotient map back to $\mathbb{CP}^5$, the three positive classes pull back to $x^3,x^4,x^5$. All positive products vanish, since their degree is at least twelve. Thus the [cohomology ring of a collapsed projective subspace](../../../../../cohomology-ring-of-a-collapsed-projective-subspace.md) in this case is the square-zero algebra $R$ on these three classes.

Now compute its [Sullivan minimal model](../../../../../sullivan-minimal-model.md) $(\Lambda V,d)$, using cohomological grading and the convention that even generators generate a [polynomial ring](../../../../../polynomial-ring.md) and odd generators an [exterior algebra](../../../../../exterior-algebra.md). Five-connectivity gives $V^j=0$ for $j\le5$. Since a minimal differential is decomposable, it cannot have a nonzero value below degree twelve. Matching [cohomology](../../../../../cohomology-split.md) through degree ten therefore forces

$$
V^6=\mathbb Qa,\quad V^8=\mathbb Qb,\quad V^{10}=\mathbb Qc,
\qquad da=db=dc=0,
$$

with no other generators in degrees at most ten. The first products must then be killed by generators

$$
\begin{aligned}
|u|&=11,&du&=a^2,\\
|v|&=13,&dv&=ab,\\
|w|&=15,&dw&=ac,\\
|t|&=15,&dt&=b^2.
\end{aligned}
$$

These follow by killing respectively the unwanted degree-twelve, degree-fourteen, and two degree-sixteen classes. Subsequent generators kill $bc,c^2$ and the resulting syzygies. For example $av-bu$ is closed of degree nineteen, so it requires a further generator of degree eighteen. Thus the full [minimal model](../../../../../sullivan-minimal-model.md) is not just the algebra on the first seven generators.

There is nevertheless a simple map from the full model to $R$: send $a,b,c$ to the three displayed classes and every other generator to zero. It is a [chain map](../../../../../chain-map.md), since every generator differential is a sum of products of positive-degree elements, and all positive products in $R$ vanish. It induces an isomorphism in [cohomology](../../../../../cohomology-split.md): the entire [cohomology](../../../../../cohomology-split.md) of $\Lambda V$ is concentrated in degrees $0,6,8,10$, and its indicated [basis](../../../../../basis.md) maps to the indicated [basis](../../../../../basis.md) of $R$. This proves [formality of a topological space](../../../../../formal-space.md) and identifies the full [minimal model](../../../../../sullivan-minimal-model.md) as a minimal resolution of $R$, rather than only matching the initial part of its [cohomology](../../../../../cohomology-split.md).

An explicit description of that full resolution is useful. Take the [free graded Lie algebra](../../../../../free-graded-lie-algebra.md)

$$
L=\mathbb L(p_5,q_7,r_9),\qquad d_L=0.
$$

Its [Chevalley–Eilenberg cochain algebra](../../../../../chevalley-eilenberg-cochains-of-a-graded-lie-algebra.md) $C^*(L)$ has one generator of degree $|\ell|+1$ for every homogeneous Lie [basis](../../../../../basis.md) word $\ell$, and its quadratic differential is dual to the bracket, with the usual graded signs. Rescaling the bracket-word duals gives exactly the generators and differentials listed above. Positive Lie degrees make this algebra Sullivan minimal. Its [cohomology](../../../../../cohomology-split.md) is $R$: the [universal enveloping algebra](../../../../../universal-enveloping-algebra.md) is $T(p,q,r)$, and the augmentation module has the exact free resolution

$$
0\longrightarrow T(p,q,r)\otimes\operatorname{span}(p,q,r)
\xrightarrow{\mathrm{multiplication}}T(p,q,r)
\longrightarrow\mathbb Q\longrightarrow0.
$$

Exactness is immediate because every nonempty tensor word has a unique last letter. Applying $\operatorname{Hom}_{T(p,q,r)}(-,\mathbb Q)$ gives just the unit and the three dual classes in total degrees $6,8,10$; products of positive classes land in an absent Ext degree two and are zero. [Chevalley–Eilenberg cochains of a graded Lie algebra](../../../../../chevalley-eilenberg-cochains-of-a-graded-lie-algebra.md) compute this Ext, so this also verifies the full model's [cohomology](../../../../../cohomology-split.md).

The [wedge sum](../../../../../wedge-sum.md) $W=S^6\vee S^8\vee S^{10}$ has the same connectivity, [cohomology ring](../../../../../cohomology-ring.md), and initial closed minimal generators. The same full-model-to-$R$ argument applies to $W$, so its [minimal model](../../../../../sullivan-minimal-model.md) is also $C^*(L)$, by uniqueness of [Sullivan minimal models](../../../../../sullivan-minimal-model.md) of quasi-isomorphic [simply connected](../../../../../simply-connected-space.md) rational cochain algebras. The [Sullivan minimal-model classification](../../../../../sullivan-minimal-model-classification.md) identifies isomorphic [minimal models](../../../../../sullivan-minimal-model.md) with the same [rational homotopy type](../../../../../rational-homotopy-type.md). Consequently

$$
\boxed{\mathbb{CP}^5/\mathbb{CP}^2\simeq_{\mathbb Q}S^6\vee S^8\vee S^{10}.}
$$

The explicit infinite minimal resolution above is shared by both spaces.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
