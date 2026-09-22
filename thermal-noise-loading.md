# Thermal noise loading

↑ **Parent:** [Thermal electrical noise](thermal-electrical-noise.md)

An external [electrical load](electrical-load.md) changes the terminal [noise](noise-signal-processing.md). Connecting a purely resistive load $R_L>0$ to the noisy [resistor](resistor.md) gives the [voltage divider](voltage-divider.md) ratio $R_L/(R+R_L)$. The source [resistor](resistor.md)'s contribution at the load is

$$
S_{v_L}^{(1)}(f)=4k_{\rm B}TR\left(\frac{R_L}{R+R_L}\right)^2.
$$

In a rectangular [signal bandwidth](signal-bandwidth.md) $B$, the [power](power.md) delivered by that source contribution to the load is

$$
P_{R\to L}=4k_{\rm B}TB\frac{RR_L}{(R+R_L)^2}\leq k_{\rm B}TB,
$$

because $(R-R_L)^2\geq0$. Equality occurs at $R_L=R$: this is matched available noise [power](power.md). Matching halves the voltage, quarters its [power spectral density](power-spectral-density.md), and gives $P_{\rm av}=k_{\rm B}TB$. Dividing the squared [open-circuit voltage](open-circuit-voltage.md) by $R$ would instead give four times this available [power](power.md).

These expressions isolate the source [resistor](resistor.md)'s contribution. A real load [resistor](resistor.md) also generates [thermal electrical noise](thermal-electrical-noise.md). At the same [temperature](temperature-split.md) its independent contribution produces the equal reverse [power](power.md) flow, so the net thermal [power](power.md) transfer is zero at [thermal equilibrium](thermal-equilibrium-split.md). For example, two equal [resistors](resistor.md) at the same [temperature](temperature-split.md) have total terminal [power spectral density](power-spectral-density.md) $2k_{\rm B}TR$, equivalent to $4k_{\rm B}T(R/2)$. One contribution alone is $k_{\rm B}TR$. The fictitious noiseless series $R$ in the [Thévenin equivalent](thevenin-equivalent.md) is not an additional physical source: adding its [noise](noise-signal-processing.md) again would double count the original [resistor](resistor.md).

## ↑ Ancestors (6)

1. [Thermal electrical noise](thermal-electrical-noise.md)
2. [Noise (signal processing)](noise-signal-processing.md)
3. [Signal](signal.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)
