<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove [full faithfulness from counit coequalizers](../../../../../../full-faithfulness-from-counit-coequalizers.md). Let $B,C\in\mathcal D$ and let $\alpha:K(B)\to K(C)$ be an [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md). Thus

$$
\alpha G\varepsilon_B=G\varepsilon_CGF\alpha.
$$

Set $u=\varepsilon_CF\alpha:FGB\to C$. Its composites with the two arrows of the printed presentation are equal: naturality of $\varepsilon$ gives

$$
u\,FG\varepsilon_B
=\varepsilon_CFG\varepsilon_CFGF\alpha
=\varepsilon_C\varepsilon_{FGC}FGF\alpha
=u\,\varepsilon_{FGB}.
$$

In the last equality we used naturality at $F\alpha$. The [coequalizer](../../../../../../coequalizer.md) property therefore gives a unique $v:B\to C$ satisfying $v\varepsilon_B=u$.

Apply $G$ to that identity. The algebra-morphism equation gives $Gv\,G\varepsilon_B=\alpha G\varepsilon_B$. The triangle identity makes $G\varepsilon_B$ a [split epimorphism](../../../../../../split-epimorphism.md) with section $\eta_{GB}$, so $Gv=\alpha$. This proves fullness of $K$.

If $v,w:B\to C$ have $Gv=Gw$, naturality gives $v\varepsilon_B=\varepsilon_CFGv=\varepsilon_CFGw=w\varepsilon_B$. The counit is epic since it is a [coequalizer](../../../../../../coequalizer.md), so $v=w$. Thus $K$ is a [faithful functor](../../../../../../faithful-functor.md). Both parallel arrows matter: the converted TeX loses the second one, $\varepsilon_{FGB}$, which is visible in the original PDF.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
