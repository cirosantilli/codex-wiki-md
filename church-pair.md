# Church pair

↑ **Parent:** [Church numeral](church-numeral.md)

With the [Church Booleans](church-boolean.md) $\mathsf T=\lambda a b.a$ and $\mathsf F=\lambda a b.b$, encode a pair by

$$
\mathsf{Pair}=\lambda a b p.pab,\qquad \mathsf{Fst}=\lambda p.p\mathsf T,\qquad \mathsf{Snd}=\lambda p.p\mathsf F.
$$

Then $\mathsf{Fst}(\mathsf{Pair}\,A\,B)\to_\beta^*A$ and the second projection similarly returns $B$. Pairing an iteration counter with a computed value implements [primitive recursion](primitive-recursion.md) using only [Church numeral](church-numeral.md) iteration.

## ↑ Ancestors (8)

1. [Church numeral](church-numeral.md)
2. [Church encoding](church-encoding.md)
3. [Lambda calculus](lambda-calculus.md)
4. [Computability theory](computability-theory.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Lambda definition of primitive recursion by pair iteration](lambda-definition-of-primitive-recursion-by-pair-iteration.md)
- [Lambda simulation of a Turing machine](lambda-simulation-of-a-turing-machine.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-20/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-25/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-120/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135/6/solution.md)
