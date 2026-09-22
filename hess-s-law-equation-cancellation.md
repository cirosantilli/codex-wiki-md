<h1 id="hess-s-law-equation-cancellation">Hess's law equation cancellation</h1>

↑ **Parent:** [Hess's law](hess-s-law.md)

Keep the [stoichiometry](stoichiometry.md) attached to the [enthalpy](enthalpy-split.md). Use the same abstract $A,B,C$ and suppose each of two entries fixes an [amount of substance](amount-of-substance.md) for every species:

$$
\begin{aligned}
R_1:&\quad 2A\longrightarrow2B, &&\Delta H_1=+36\,\mathrm{kJ},\\
R_2:&\quad C\longrightarrow B, &&\Delta H_2=+25\,\mathrm{kJ}.
\end{aligned}
$$

Here each unit coefficient represents one [mole](mole-unit.md) on the common basis. To obtain $A\to C$, halve $R_1$ and reverse $R_2$. Adding those transformed [chemical equations](chemical-equation.md) gives

$$
\begin{aligned}
\tfrac12R_1:&\quad A\longrightarrow B, &&\tfrac12\Delta H_1=+18\,\mathrm{kJ},\\
-R_2:&\quad B\longrightarrow C, &&-\Delta H_2=-25\,\mathrm{kJ},\\
\text{sum}:&\quad A+B\longrightarrow B+C, &&\Delta H=-7\,\mathrm{kJ}.
\end{aligned}
$$

The equal amounts of $B$ on opposite sides cancel, leaving $A\to C$. Doubling this final [chemical equation](chemical-equation.md) would give $2A\to2C$ and $\Delta H=-14\,\mathrm{kJ}$; its change per [mole](mole-unit.md) of $A$ would remain $-7\,\mathrm{kJ\,mol^{-1}}$.

More generally, write each [chemical equation](chemical-equation.md) as a [stoichiometric vector](stoichiometric-vector.md) $\boldsymbol\nu_j$, with negative entries for [reactants](reactant.md) and positive entries for [reaction products](product-chemistry.md). Finding coefficients $a_j$ with $\boldsymbol\nu_{\rm target}=\sum_j a_j\boldsymbol\nu_j$ also gives $\Delta H_{\rm target}=\sum_j a_j\Delta H_j$, using compatible state and amount conventions. An identical [chemical species](chemical-species.md) cancels only with the same [thermodynamic phase](thermodynamic-phase.md) and composition conditions. A leftover [water](water.md) or [dilution](dilution.md) step is a real part of the balance.

## ↑ Ancestors (4)

1. [Hess's law](hess-s-law.md)
2. [Thermochemistry](thermochemistry.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)
