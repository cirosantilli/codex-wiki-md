<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $T:\mathcal C^{\mathrm{op}}\times\mathcal C\to\mathcal D$. A [categorical end](../../../../../../end-of-a-functor.md) is an object $E$ with [morphisms](../../../../../../morphism.md) $e_A:E\to T(A,A)$ satisfying, for every $f:A\to B$,

$$
T(1_A,f)e_A=T(f,1_B)e_B.
$$

It is universal among such families: any $x_A:X\to T(A,A)$ satisfying the same equations is uniquely $e_Ah$ for one $h:X\to E$. This is a universal [dinatural transformation](../../../../../../dinatural-transformation.md) from the constant value $E$, and is written $E=\int_A T(A,A)$.

Dually a [categorical coend](../../../../../../coend-of-a-functor.md) is $Q$ with [morphisms](../../../../../../morphism.md) $j_A:T(A,A)\to Q$ satisfying

$$
j_BT(1_B,f)=j_AT(f,1_A):T(B,A)\to Q.
$$

Any family $x_A:T(A,A)\to X$ satisfying these equations is uniquely $h j_A$ for one $h:Q\to X$. Write $Q=\int^A T(A,A)$. For small $\mathcal C$, the [categorical end](../../../../../../end-of-a-functor.md) can be constructed as the [equalizer](../../../../../../equaliser.md) of $\prod_AT(A,A)\rightrightarrows\prod_{f:A\to B}T(A,B)$ when these objects exist. The [categorical coend](../../../../../../coend-of-a-functor.md) is the [coequalizer](../../../../../../coequalizer.md) of $\coprod_{f:A\to B}T(B,A)\rightrightarrows\coprod_AT(A,A)$ when those objects exist. The two [morphisms](../../../../../../morphism.md) impose exactly the displayed equations for a [dinatural transformation](../../../../../../dinatural-transformation.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
