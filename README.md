# Critical two-point functions and finite-size scaling in the Ising and $\phi^4$ models

Research manuscripts by Jiwoon Park on critical correlations in the square-lattice $\phi^4$ model and the spread-out Ising model, and on finite-size scaling in Ising boxes with free boundaries. The manuscripts were prepared with human and AI contributions and are subject to revision. See the individual manuscripts for AI statements.

[![DOI](https://zenodo.org/badge/1449114649.svg)](https://doi.org/10.5281/zenodo.24167641)

## Finite-size scaling with free boundaries

The two papers in [FSS](FSS/) study the spread-out Ising model on a cube of side $n$ and volume $V=n^d$, for $d\in\{1,2,3,4\}$ and sufficiently large fixed spread radius $R$. The operator $(-\Delta_R)^{d/4}$ places each model at its upper critical dimension.

### Pseudocritical point and susceptibility

The first paper constructs a renormalisation group flow with free boundary condition. It defines a finite-volume pseudocritical inverse temperature $\tau_n^{\mathrm{pc}}$ by requiring the effective potential of the principal mode to have zero curvature at the origin. At this point, the susceptibility of the total spin satisfies

$$
\chi_n^F(\tau_n^{\mathrm{pc}})
= \frac{1}{V}{Var}_{\tau_n^{\mathrm{pc}}}^F\!\left(\sum_{x\in\Lambda_n}\sigma_x\right)
\asymp \sqrt{V\log V}.
$$

In four dimensions, this gives $n^2\sqrt{\log n}$. The companion paper shows that $\tau_n^{\mathrm{pc}}\to\tau_c$ and that the shift $\tau_n^{\mathrm{pc}}-\tau_c$ is at least $c_{d,R}n^{-d/2}$ for all sufficiently large $n$.

[Read the susceptibility paper (PDF)](FSS/FSS_FBC-dim-extension.pdf) · [LaTeX source](FSS/FSS_FBC-dim-extension.tex) · [Abstract and main theorem](https://jiwoon-park-math.github.io/free-boundary-pseudocritical-point.html)

### Gaussian and non-Gaussian fluctuations

The companion paper tests the spin field against a smooth, nonzero function $F$ vanishing on the boundary of the unit cube. With lattice weights $(n+1)^{-d/2}F(x/(n+1))$, the variance and limiting law of the spin sum at $\tau_n^{\mathrm{pc}}$ depend on the overlap of $F$ with the continuum ground state $w$.

| Test function | Variance of the spin sum (order) | Limiting law of the standardised spin sum |
| --- | --- | --- |
| Nonzero overlap with $w$ | $n^{d/2}\sqrt{\log n}$ | Quartic law, rescaled to unit variance |
| Orthogonal to $w$ | $n^{d/2}$ | Standard Gaussian |

For example, in $d=4$ the lowest sine mode $(1,1,1,1)$ has a quartic limit, while the $(3,1,1,1)$ sine mode has a Gaussian limit.

[Read the spin observables paper (PDF)](FSS/FSS_FBC-obs-extension.pdf) · [LaTeX source](FSS/FSS_FBC-obs-extension.tex) · [Abstract and main theorem](https://jiwoon-park-math.github.io/free-boundary-spin-observables.html)

## Infinite-volume critical two-point functions

### Square-lattice $\phi^4$ at strong coupling

For the nearest-neighbour model with single-site weight proportional to $e^{-g(\phi^2-1)^2}$ and sufficiently large $g$, the critical free two-point function has the Ising decay exponent $1/4$.

$$
\langle \phi_0\phi_x\rangle^0_{\beta_c(g)}
\sim C_g |x|^{-1/4}, \qquad C_g>0, \quad |x|\to\infty.
$$

[Read the paper (PDF)](critical_phi42/critical_phi42.pdf) · [LaTeX source](critical_phi42/critical_phi42.tex) · [Abstract and main theorem](https://jiwoon-park-math.github.io/critical-phi4.html)

### Fractional spread-out Ising models at their upper critical dimension

For $d\in\{1,2,3,4\}$ and sufficiently large fixed $R$, the critical free two-point function of the Ising model with operator $(-\Delta_R)^{d/4}$ has the asymptotic form

$$
\langle \sigma_0\sigma_x\rangle^f_{\tau_c}
\sim C_{d,R}|x|^{-d/2}, \qquad C_{d,R}>0, \quad |x|\to\infty.
$$

In $d=4$ the operator is the finite-range spread-out Laplacian and the decay is $C_{4,R}|x|^{-2}$.

[Read the paper (PDF)](fractional_spread_out_ising_rg/spread_out_ising_rg.pdf) · [LaTeX source](fractional_spread_out_ising_rg/spread_out_ising_rg.tex) · [Abstract and main theorem](https://jiwoon-park-math.github.io/fractional-spread-out-ising.html)
