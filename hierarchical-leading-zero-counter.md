# Hierarchical leading-zero counter

↑ **Parent:** [Count leading zeros](count-leading-zeros.md)

For a block of $2^k$ [bits](bit.md), encode its [count leading zeros](count-leading-zeros.md) result as a zero flag $z$ followed by $k$ low count [bits](bit.md) $r$. An all-zero block has $(z,r)=(1,0)$; otherwise $z=0$. Two half-block encoders supply flags $z_H,z_L$ and low counts $h,\ell$. Combine them using $z=z_H\land z_L$, $r_{k-1}=z_H\land\neg z_L$, and $r_i=\operatorname{mux}(z_H,h_i,\ell_i)$ for $i<k-1$. A one-[bit](bit.md) leaf has $z=\neg x$ and no low count [bits](bit.md). Checking whether the upper half is nonzero, only the lower half is nonzero, or both halves are zero proves the formula.

All count [bits](bit.md) are selected in parallel, so $D(n)=D(n/2)+O(1)$ for [circuit depth](depth-of-a-boolean-circuit.md). The [circuit size](circuit-size.md) satisfies $S(n)=2S(n/2)+O(\log n)$; summing the work over levels gives $S(n)=O(n)$. Sharing the all-zero flags avoids a serial [adder](adder.md) along the critical path.

## ↑ Ancestors (8)

1. [Count leading zeros](count-leading-zeros.md)
2. [Combinational logic](combinational-logic.md)
3. [Boolean circuit](boolean-circuit.md)
4. [Circuit complexity](circuit-complexity.md)
5. [Computational complexity theory](computational-complexity-theory.md)
6. [Theoretical computer science](theoretical-computer-science-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/1/d/solution.md)
