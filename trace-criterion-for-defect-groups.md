# Trace criterion for defect groups

↑ **Parent:** [Defect group of a block](defect-group-of-a-block.md)

For a $p$-subgroup $D$ of a finite [group](group-split.md) $G$, set $I_D=\operatorname{Tr}_D^G((kG)^D)$, a [transfer ideal of conjugation-fixed elements](transfer-ideal-of-conjugation-fixed-elements.md) in $Z(kG)$. A [block of a group algebra](block-of-a-group-algebra.md) idempotent $b$ lies in $I_D$ if and only if a [defect group of a block](defect-group-of-a-block.md) of $b$ is conjugate to a subgroup of $D$. In particular, defect groups can equivalently be defined as minimal subgroups $D$ with $b\in I_D$.

Here is a proof using the [Brauer morphism](brauer-morphism.md). A subgroup of smallest order with $b\in I_D$ exists, since a [Sylow subgroup](sylow-subgroup.md) $P$ gives $b=\operatorname{Tr}_P^G(b/[G:P])$. Write $b=\operatorname{Tr}_D^G(a)$ and replace $a$ by $ba$. If $\operatorname{Br}_D(b)=0$, then $ba$ belongs to the kernel of the Brauer morphism, which is the sum of proper-subgroup relative traces. Hence $b\in\sum_{Q<D}I_Q$. The algebra $bZ(kG)$ is a commutative [Artinian ring](artinian-ring.md) and a [local ring](local-ring.md), so multiplying this equality by $b$ forces some ideal $bI_Q$ to contain its identity $b$. This contradicts minimality. On the other hand, $\operatorname{Br}_E(I_D)=0$ unless $E$ is conjugate into $D$: the $E$-action on $G/D$ has no fixed coset otherwise, and nonfixed orbit sizes vanish in characteristic $p$. Thus these minimal subgroups are precisely the maximal subgroups with nonzero Brauer image. They are all conjugate. Trace transitivity proves the stated criterion for larger $D$.

## ↑ Ancestors (8)

1. [Defect group of a block](defect-group-of-a-block.md)
2. [Block of a group algebra](block-of-a-group-algebra.md)
3. [Modular representation theory](modular-representation-theory.md)
4. [Representation theory](representation-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Brauer morphism on a defect transfer ideal](brauer-morphism-on-a-defect-transfer-ideal.md)
- [Modules in a block are projective relative to its defect group](modules-in-a-block-are-projective-relative-to-its-defect-group.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-5/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-5/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-3/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-4/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-138/6/a/solution.md)
