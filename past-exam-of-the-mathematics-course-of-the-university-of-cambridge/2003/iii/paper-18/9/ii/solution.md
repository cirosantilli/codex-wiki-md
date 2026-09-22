<h1 id="9/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $T=GF$, define the [Eilenberg-Moore comparison functor](../../../../../../eilenberg-moore-comparison-functor.md)

$$
\boxed{K(D)=(GD,a_D),\qquad a_D=G\varepsilon_D,\qquad K(h)=Gh.}
$$

The algebra unit law is a triangle identity. Naturality of the counit at $\varepsilon_D$ gives its algebra associativity law; naturality at $h:D\to E$ gives $Gh\,a_D=a_E T(Gh)$, making $K(h)$ an algebra morphism.

Suppose first that $G$ reflects G-split [coequalizers](../../../../../../coequalizer.md). For every $D$, consider the counit presentation

$$
FGFGD\underset{FG\varepsilon_D}{\overset{\varepsilon_{FGD}}{\rightrightarrows}}FGD\xrightarrow{\varepsilon_D}D.
$$

It equalizes the pair by counit naturality. After applying $G$ it becomes $T^2GD\rightrightarrows TGD\xrightarrow{a_D}GD$, with parallel maps $\mu_{GD},T(a_D)$. This is split: take $s=\eta_{GD}$ and $t=\eta_{TGD}$. The identities $a_Ds=1$, $\mu_{GD}t=1$ and $T(a_D)t=\eta_{GD}a_D$ follow from the algebra law, a [monad](../../../../../../monad.md) unit law, and naturality of $\eta$. Reflection therefore makes $\varepsilon_D$ a [coequalizer](../../../../../../coequalizer.md) in $\mathcal D$.

For faithfulness, if $Gh=Gk$ then naturality gives $h\varepsilon_D=\varepsilon_EFGh=\varepsilon_EFGk=k\varepsilon_D$. [Coequalizers](../../../../../../coequalizer.md) are epic, so $h=k$.

For fullness, let $\alpha:GD\to GE$ be an algebra morphism, so $\alpha a_D=a_E T\alpha$. Put $h_0=\varepsilon_EF\alpha:FGD\to E$. Its two composites with the counit-presentation pair are equal: by counit naturality they are $\varepsilon_EF(a_ET\alpha)$ and $\varepsilon_EF(\alpha a_D)$. Hence there is a unique $h:D\to E$ with $h\varepsilon_D=h_0$. Applying $G$ gives $Gh\,a_D=a_ET\alpha=\alpha a_D$. Since $a_D$ is split epic, $Gh=\alpha$. This proves full faithfulness directly by descent.

Conversely suppose $K$ is full and faithful. We need the following explicit algebra lifting fact. For algebra morphisms $f,g:(A,a)\rightrightarrows(B,b)$ with a split underlying [coequalizer](../../../../../../coequalizer.md) $q:B\to Q$, the arrow $qb:TB\to Q$ equalizes $Tf,Tg$. The split diagram is preserved by $T$, so $Tq$ is their [coequalizer](../../../../../../coequalizer.md) and there is a unique $c:TQ\to Q$ with $cTq=qb$. Precomposing the unit equation with the [epimorphism](../../../../../../epimorphism.md) $q$ gives $c\eta_Qq=q$; precomposing the associativity equation with the [epimorphism](../../../../../../epimorphism.md) $T^2q$ gives equality by $bT(b)=b\mu_B$. Thus $c$ is an algebra action. If an algebra map $h:B\to(Z,z)$ equalizes $f,g$, its unique underlying factor $k:Q\to Z$ satisfies $kcTq=hb=zTh=zTkTq$. Cancelling $Tq$ shows $kc=zTk$. This proves [monad algebra forgetful functor creates split coequalizers](../../../../../../monad-algebra-forgetful-functor-creates-split-coequalizers.md).

Now take any existing equalizing arrow $e:B\to D$ in $\mathcal D$ whose image is such a [coequalizer](../../../../../../coequalizer.md). The lifting fact makes the unique compatible action on $GD$ its already given action $a_D$, since $Ke$ preserves that action. Hence $Ke$ is a [coequalizer](../../../../../../coequalizer.md) of $Kf,Kg$ in the algebra category. For any arrow $h:B\to Z$ equalizing the pair, its unique algebra factor $KD\to KZ$ lifts to an arrow $D\to Z$ by fullness of $K$; faithfulness gives its factorization equation and uniqueness. Therefore $e$ is a [coequalizer](../../../../../../coequalizer.md) in $\mathcal D$. We have proved the [full comparison and reflection of split coequalizers](../../../../../../full-comparison-and-reflection-of-split-coequalizers.md) equivalence

$$
\boxed{K\text{ is full and faithful}\iff G\text{ reflects G-split coequalizers}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [9](../../9.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
