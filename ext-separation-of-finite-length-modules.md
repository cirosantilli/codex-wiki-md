# Ext separation of finite-length modules

↑ **Parent:** [Ext functor](ext-functor.md)

Partition the isomorphism classes of [simple modules](irreducible-module.md) into two sets $\mathcal C_1,\mathcal C_2$, with $\operatorname{Ext}^1(S,T)=\operatorname{Ext}^1(T,S)=0$ whenever $S,T$ lie in different sets. Every [module](module-mathematics.md) $M$ of finite [composition length](composition-length.md) then has a unique decomposition $M=U_1\oplus U_2$ into its largest [submodules](submodule.md) whose [Jordan–Hölder factors](jordan-holder-factor.md) belong to the respective sets.

For a simple $S\in\mathcal C_1$ and a finite-length $N$ with factors in $\mathcal C_2$, induction through the long exact sequence of the [Ext functor](ext-functor.md) gives $\operatorname{Ext}^1(S,N)=0$. Induct on the length of $M$: take $0\to N\to M\to S\to0$, split $N=N_1\oplus N_2$, and suppose $S\in\mathcal C_1$. The quotient extension $0\to N_2\to M/N_1\to S\to0$ splits. The inverse image of its $S$-summand complements $N_2$ in $M$ and has only factors in $\mathcal C_1$. Finally, Hom between modules with factors in different sets is zero, since any nonzero image would have a factor in both sets. Projecting any proposed [submodule](submodule.md) to the opposite summand therefore proves maximality and uniqueness.

## ↑ Ancestors (7)

1. [Ext functor](ext-functor.md)
2. [Hom functor](hom-functor.md)
3. [Homological algebra](homological-algebra.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Ext-connected components determine blocks](ext-connected-components-determine-blocks.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-138/5/a/solution.md)
