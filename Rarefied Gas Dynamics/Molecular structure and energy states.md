
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [Diatomic molecules](#diatomic-molecules)
- [Internal energy distribution function](#internal-energy-distribution-function)

<!-- /code_chunk_output -->


# Diatomic molecules

The order of magnitude **electronic energy**$ \varepsilon_e $ is
$$ \varepsilon_e \sim \frac{h^2}{md^2}$$

where $h$ is the Planck constant; $m$ is the mass of the electron; $d$ is the linear scale of the molecule.
The order of magnitude **vibratioinal energy**$ \varepsilon_v $ is
$$ \varepsilon_v \sim \sqrt{\frac{m}{M}} \varepsilon_e $$

where $M$ is the mass of the nucleus.
The order of magnitude **rotational energy**$ \varepsilon_r $ is
$$ \varepsilon_r \sim \frac{m}{M} \varepsilon_e $$

As the mass $M$ of the nucleus is four orders of magnitude larger than the mass $m$ of the electron, $M/m \sim 10^4$, one can ascertain, that $\varepsilon_v$ is two orders of magnitude smaller than $\varepsilon_e$, and $\varepsilon_r$ is another two orders of magnitudes smaller than $\varepsilon_v$.

Any energy level represents the energy of the molecule of energy $\varepsilon$, and corresponds to certain electronic energy level, certain vibrational quantum number $n$ and certain rotational quantum number $J$.

When the interaction between the various energyvmodes are neglected, the internal energy of molecules can be presented as the sum of electronic energy $\varepsilon$, vibrational energy $\varepsilon_v$ and rotational energy $\varepsilon_r$, if add the kinetic energy $\varepsilon_{tr}$ of the motion of molecules, the energy of a molecule can be presented as
$$ \varepsilon = \varepsilon_e+\varepsilon_v+\varepsilon_r+\varepsilon_{tr} $$

# Internal energy distribution function

The **specific translational energy**, or the internal energy associated with the translational energy per unit mass, is
$$ e_{tr}=\frac{3}{2}RT $$

The **specific rotational energy** is
$$ e_r=RT $$

The **specific vibrational energy** is
$$ e_v = \frac{R\Theta_v}{e^{\Theta_v/T}-1} $$

where $\Theta_v=h\nu/k$.
If suppose the vibrational energy has $\zeta_v$ degrees of freedom, then according to the **principle of equipartition of energies** the specific vibratioinal energy can be written
$$ e_v=\frac{\zeta_v}{2}RT \equiv \frac{\zeta_v}{2}\frac{k}{m}T = \frac{R\Theta_v}{e^{\Theta_v/T}-1} $$

It is seen that the expression of $\zeta_v$ is given by
$$ \zeta_v=\frac{2\Theta_v/T}{e^{\Theta_v/T}-1}$$

Only at very high temperature $\Theta_v \to 2$. Thus it can be seen, the contribution of the translational motion and the rotation of molecules to the specific heat is $(5/2)R$, and the vibrational specific heat changes with temperature.

The distribution function of energy $\varepsilon$ with $\zeta$ degrees of freedom is
$$ f(\varepsilon)=\frac{1}{\Gamma(\zeta/2)}\frac{\varepsilon^{\frac{\zeta}{2}-1}}{(kT)^{\zeta/2}}e^{-\varepsilon/kT}$$

This is certainly true for vibrational energy $\varepsilon_v$ with $\zeta_v$ degrees of freedom.