<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [gravity anomaly](../../../../../gravity-anomaly.md) is the difference between observed gravitational acceleration and a specified reference prediction after defined reductions. A [free-air gravity anomaly](../../../../../free-air-gravity-anomaly.md), a [Bouguer gravity anomaly](../../../../../bouguer-gravity-anomaly.md), and a residual local [gravity anomaly](../../../../../gravity-anomaly.md) differ because they remove different reference contributions. State the reference [ellipsoid](../../../../../ellipsoid.md), datum, reference [density](../../../../../density.md), and regional trend before interpreting an anomaly as a subsurface [geophysical density contrast](../../../../../geophysical-density-contrast.md).

On land, tie [gravimeter](../../../../../gravimeter.md) observations to a gravity base, calibrate them, correct instrumental drift and Earth tides, and determine station [latitude](../../../../../geographical-latitude.md) and elevation accurately. Subtract latitude-dependent normal gravity $\gamma(\varphi)$. Reduce to the reference elevation using a positive [free-air correction](../../../../../free-air-correction.md) for a station above that datum: about $+0.3086h\ \mathrm{mGal}$ for $h$ in metres. A simple [Bouguer gravity anomaly](../../../../../bouguer-gravity-anomaly.md) then subtracts attraction of the intervening rock slab and adds the conventional [terrain correction](../../../../../terrain-correction.md):

$$
\Delta g_B\simeq g_{\mathrm{obs,corr}}-\gamma(\varphi)+0.3086h-2\pi G\rho_{\mathrm{ref}}h+C_{\mathrm{terrain}},
$$

with all acceleration terms expressed consistently. In SI units $1\ \mathrm{mGal}=10^{-5}\ \mathrm{m\,s^{-2}}$.

At sea, also correct vessel-motion effects, especially the [Eötvös correction](../../../../../eotvos-correction.md) from east–west vessel motion and Earth rotation, and vertical ship acceleration; average or filter the moving-platform data appropriately. GPS navigation and tide information specify position and measurement height. Sea-surface measurements give a marine [free-air gravity anomaly](../../../../../free-air-gravity-anomaly.md) after motion, latitude, tide and height reductions. A marine [Bouguer gravity anomaly](../../../../../bouguer-gravity-anomaly.md) additionally allows for measured [bathymetry](../../../../../bathymetry.md) and the replacement of low-density [water](../../../../../water.md) by reference [rock](../../../../../rock-geology.md); the simple water-column replacement correction is positive, $2\pi G(\rho_{\mathrm{ref}}-\rho_w)H$, relative to the sea-surface free-air value. A consistent three-dimensional bathymetric correction is preferable near irregular coasts. Remove a justified broad regional field if the intended quantity is a residual anomaly of the local body.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
