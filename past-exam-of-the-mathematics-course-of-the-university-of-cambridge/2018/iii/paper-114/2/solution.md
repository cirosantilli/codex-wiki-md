<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $v$ for the cone vertex. The quotient is the [topological mapping cone](../../../../../mapping-cone-topology.md) $C_f=Y\cup_f CX$. First assume $X\ne\varnothing$, as is implicit in having this vertex; a map then also forces $Y\ne\varnothing$.

Take the open cover consisting of the image of $X\times[0,2/3)$ and the image of $Y\sqcup(X\times(1/3,1])$. Denote these sets by $U,V$. The first contracts to $v$, the second has a [deformation retraction](../../../../../deformation-retraction.md) onto $Y$, and $U\cap V\cong X\times(1/3,2/3)$ retracts onto $X$. Under these identifications the two inclusion maps induce the zero map into positive-degree [homology](../../../../../homology-split.md) of $U$ and $f_*$ into the homology of $V$. The [Mayer–Vietoris theorem](../../../../../mayer-vietoris-sequence.md) consequently gives, in positive degrees,

$$
\boxed{\cdots\longrightarrow\widetilde H_{q+1}(Z;G)
\longrightarrow H_q(X;G)\xrightarrow{f_*}H_q(Y;G)
\longrightarrow\widetilde H_q(Z;G)\longrightarrow\cdots.}
$$

The same assertion holds in degree zero, but needs care: the ordinary Mayer-Vietoris map is

$$
H_0(X;G)\longrightarrow H_0(Y;G)\oplus G,
\qquad a\longmapsto(f_*a,-\varepsilon_Xa).
$$

Since $\varepsilon_Yf_*a=\varepsilon_Xa$, its kernel equals $\ker f_*$. On quotienting $H_0(Z;G)$ by the direct summand $G[v]$, its cokernel becomes $\operatorname{coker}f_*$. That quotient is canonically identified with [reduced homology](../../../../../reduced-homology.md) by subtracting the augmentation times $[v]$. Thus the last nonzero part is

$$
\widetilde H_1(Z;G)\longrightarrow H_0(X;G)\xrightarrow{f_*}H_0(Y;G)
\longrightarrow\widetilde H_0(Z;G)\longrightarrow0.
$$

In particular the map from $H_0(Y;G)$ sends a component class $[y]$ to $[y]-[v]$. This proves the [mapping cone exact sequence](../../../../../mapping-cone-exact-sequence.md); finite generation of $G$ is not needed for this construction.

There is a literal empty-space exception in the printed hypotheses. If $X=\varnothing$ and $Y$ is a point, the given quotient is just $Y$, and the asserted degree-zero exact sequence would be $0\to G\to0$. Thus the displayed reduced sequence presupposes nonempty $X$. It holds also for empty $X$ if one defines its cone to include a new isolated vertex. The later homology-isomorphism claim itself remains true for empty finite complexes, with the cases involving one empty complex dealt with directly in degree zero.

Now take nonempty finite [CW complexes](../../../../../cw-complex.md) $X,Y$. Put $A_q=\widetilde H_q(Z;\mathbb Z)$. The exact sequence gives

$$
0\longrightarrow\operatorname{coker}(f_*:H_q(X)\to H_q(Y))
\longrightarrow A_q\longrightarrow
\ker(f_*:H_{q-1}(X)\to H_{q-1}(Y))\longrightarrow0,
$$

where $H_{-1}=0$. All $A_q$ are [finitely generated abelian groups](../../../../../finitely-generated-abelian-group.md), since the groups for $X,Y$ are finitely generated. Moreover, by exactness,

$$
f_*\text{ is an integral homology isomorphism}\quad\Longleftrightarrow\quad A_q=0\text{ for every }q.
$$

The reduced [universal coefficient theorem for homology](../../../../../universal-coefficient-theorem-for-homology.md) gives

$$
0\longrightarrow A_q\otimes\mathbb F_p
\longrightarrow\widetilde H_q(Z;\mathbb F_p)
\longrightarrow\operatorname{Tor}^{\mathbb Z}_1(A_{q-1},\mathbb F_p)\longrightarrow0.
$$

If all $A_q$ vanish, so does the middle term for every prime, and the exact sequence with coefficients proves that $f_*$ is an isomorphism modulo every prime. Conversely, those isomorphisms imply that the middle terms vanish, hence $A_q\otimes\mathbb F_p=0$ for every prime $p$. By the [Fundamental theorem of finitely generated abelian groups](../../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md), a nonzero free summand would survive modulo every prime, and a cyclic torsion summand would survive modulo a prime dividing its order. Thus $A_q=0$ for every $q$, proving

$$
\boxed{f_*:H_*(X;\mathbb Z)\xrightarrow{\sim}H_*(Y;\mathbb Z)
\quad\Longleftrightarrow\quad
f_*:H_*(X;\mathbb F_p)\xrightarrow{\sim}H_*(Y;\mathbb F_p)\text{ for every prime }p.}
$$

This argument uses the exact sequence to obtain finite generation; it does not assume in advance that the cone of an arbitrary continuous map is a finite [CW complex](../../../../../cw-complex.md).

Finally suppose $f$ is a [cellular map](../../../../../cellular-map.md). Keep the cells of $Y$, add the vertex $v$, and add a $(q+1)$-cell for the cone on every $q$-cell of $X$. Its top face attaches to $Y$ through $f$, and its other faces attach to cones on lower-dimensional cells. The cellular condition puts these attachments in the appropriate skeleton. This constructs a [finite CW complex](../../../../../finite-cw-complex.md) structure on $Z$.

Let $A_*=C_*^{\mathrm{cell}}(X)$ and $B_*=C_*^{\mathrm{cell}}(Y)$ be the ordinary [cellular chain complexes](../../../../../cellular-chain-complex.md), with $A_{-1}=0$. Orient each coned cell so that its boundary has the form $f_\#(e)-c(d_Ae)$. Using $[y]-[v]$ as the reduced generator for each vertex of $Y$ gives

$$
\boxed{\widetilde C_q^{\mathrm{cell}}(Z)=B_q\oplus A_{q-1},\qquad
D_q(y,x)=(d_By+f_\#x,-d_Ax)\quad(q\geq0).}
$$

In particular $\widetilde C_0^{\mathrm{cell}}(Z)=B_0$, and the boundary of a cone edge is its image vertex minus $v$. The [chain map](../../../../../chain-map.md) identity $d_Bf_\#=f_\#d_A$ gives

$$
D^2(y,x)=(d_B^2y+d_Bf_\#x-f_\#d_Ax,d_A^2x)=0.
$$

This is the [cellular chain complex of a mapping cone](../../../../../cellular-chain-complex-of-a-mapping-cone.md), equivalently the algebraic [mapping cone](../../../../../mapping-cone-homological-algebra.md) with the displayed summand and sign conventions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
