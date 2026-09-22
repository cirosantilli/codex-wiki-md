<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If $L\in\operatorname{Pic}^0(X)$, part (iii) makes $\Lambda(L)$ trivial. Pulling it back along $(f,g):Y\to X\times X$ gives

$$
\boxed{(f+g)^*L\simeq f^*L\otimes g^*L.}
$$

Taking $Y=X$, $f=\operatorname{id}_X$, and $g=i$, where $i$ is inversion, gives

$$
\mathcal O_X\simeq L\otimes i^*L,
\qquad
\boxed{i^*L\simeq L^\vee.}
$$

Induction with $f=[n]$ and $g=\operatorname{id}_X$ proves $[n]^*L\simeq L^{\otimes n}$ for $n\ge0$; combining this with inversion proves

$$
\boxed{[n]^*L\simeq L^{\otimes n}\quad(n\in\mathbb Z).}
$$

Conversely, suppose $i^*L\simeq L^\vee$. For $M=\phi_L(x)$, part (ii) gives $M\in\operatorname{Pic}^0(X)$, so the result just proved yields $i^*M\simeq M^\vee$. On the other hand,

$$
\phi_{i^*L}(x)=i^*\phi_L(-x)=i^*(M^\vee)\simeq M,
$$

whereas $i^*L\simeq L^\vee$ gives $\phi_{i^*L}(x)=\phi_{L^\vee}(x)=M^\vee$. Hence $M^{\otimes2}$ is trivial for every $x$, so $\phi_{L^{\otimes2}}$ is trivial and $L^{\otimes2}\in\operatorname{Pic}^0(X)$. The torsion-freeness proved in part (ii) now implies

$$
\boxed{L\in\operatorname{Pic}^0(X).}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
