# Complementary CMOS network duality

↑ **Parent:** [CMOS](cmos.md)

For an [NMOS transistor](nmos-transistor.md) network described by a series-parallel expression in conducting inputs, replace series by parallel, parallel by series, and each device by a [PMOS transistor](pmos-transistor.md) driven by the same input. [De Morgan's laws](de-morgan-s-laws.md) show recursively that the resulting [pull-up network](pull-up-network.md) conducts exactly when the original [pull-down network](pull-down-network.md) does not. This proves complementary rail connections for stable binary inputs in the ideal static model. Factoring a [Boolean function](boolean-function.md) before constructing its dual can remove duplicated devices: $ab\lor bc=b(a\lor c)$ needs three lower and three upper devices, instead of four of each. Physical switching transients, device sizing and delays are additional engineering questions.

## ↑ Ancestors (7)

1. [CMOS](cmos.md)
2. [MOSFET](mosfet.md)
3. [Field-effect transistor](field-effect-transistor.md)
4. [Transistor](transistor.md)
5. [Semiconductor](semiconductor-split.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/3/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/3/c/solution.md)
