<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Since $Y$ is a maximal [matroid independent set](../../../../../../independent-set-of-a-matroid.md) in $Z$, augmentation gives $r(Y)=|Y|=r(Z)$. For any $x\in X$, the [rank of a matroid](../../../../../../rank-of-a-matroid.md) of $Z+x$ equals that of $Y+x$. Indeed, if $x\notin Z$, either $Y+x$ is independent and has the largest possible size $|Y|+1$, or it is dependent and $Y$ is still maximal in $Z+x$: no element of $Z\setminus Y$ can be added, and neither can $x$. If $x\in Z$, both ranks are simply $|Y|$.

Consequently $r(Y+x)=r(Y)$ if and only if $r(Z+x)=r(Z)$, which proves **$\sigma(Y)=\sigma(Z)$** for the [closure of a matroid](../../../../../../closure-of-a-matroid.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Combinatorial optimisation](../../../../combinatorial-optimisation-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
