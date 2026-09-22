# Charge neutrality with partial donor ionization

↑ **Parent:** [Semiconductor doping](semiconductor-doping.md)

For a nondegenerate [semiconductor](semiconductor-split.md) with donor density $N_D$, no acceptors, and donor energy $E_D=E_c-E_b$, an occupied donor has two electron spin states while an empty donor has one. Its ionized fraction is therefore $N_D^+/N_D=[1+2e^{(E_F-E_D)/(k_BT)}]^{-1}$. The conduction-band relation $n=N_ce^{(E_F-E_c)/(k_BT)}$ gives $N_D^+=N_D/[1+(2n/N_c)e^{E_b/(k_BT)}]$. Combining [charge neutrality](charge-neutrality.md), $n-p=N_D^+$, with the [semiconductor mass-action law](semiconductor-mass-action-law.md), $np=n_i^2$, proves the displayed equation.

Its left side increases strictly for $n>0$ and its right side decreases, so there is one physical solution, with $n\geq n_i$. In the freeze-out regime, holes are negligible and solving the quadratic gives $n=2N_D/[1+\sqrt{1+(8N_D/N_c)e^{E_b/(k_BT)}}]$. Strong [dopant freeze-out](dopant-freeze-out.md) reduces this to $n\simeq\sqrt{N_DN_c/2}\,e^{-E_b/(2k_BT)}$. An extrinsic plateau requires $(2N_D/N_c)e^{E_b/(k_BT)}\ll1$ and $n_i\ll N_D$, not simply $k_BT\gg E_b$.

**Table of contents**

- [Full ionization versus isolated donor occupation](full-ionization-versus-isolated-donor-occupation.md)

## ↑ Ancestors (4)

1. [Semiconductor doping](semiconductor-doping.md)
2. [Semiconductor](semiconductor-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-2/a10/b/ii/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006/section-b/b5/solution.md)
