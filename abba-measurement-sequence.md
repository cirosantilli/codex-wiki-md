# ABBA measurement sequence

↑ **Parent:** [Differential length comparator](differential-length-comparator.md)

Alternating sample and reference readings can suppress instrument drift. In this original four-reading model, measure objects $A,B,B,A$ at equally spaced times $0,\Delta t,2\Delta t,3\Delta t$. Assume the objects are stable during that short sequence and each reading is its object's [length](length.md) plus the same [affine function](affine-function.md) of time, $a+bt$. Then

$$
\widehat{B-A}=\frac{y_1+y_2-y_0-y_3}{2}=L_B-L_A,
$$

because both pairs have mean time $3\Delta t/2$. The constant offset and linear drift cancel. With a further drift term $ct^2$, direct substitution instead leaves bias $-2c\Delta t^2$. A shorter sequence reduces that term, but neither this ordering nor averaging corrects unequal [temperatures](temperature-split.md), sample changes or reference [measurement uncertainty](measurement-uncertainty.md). This is a modern illustrative protocol; the historical account below establishes alternation, without attributing this particular four-reading sequence to [Charles-Édouard Guillaume](charles-edouard-guillaume.md).

## ↑ Ancestors (5)

1. [Differential length comparator](differential-length-comparator.md)
2. [Dimensional metrology](dimensional-metrology.md)
3. [Metrology](metrology.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-d/d13/b/solution.md)
