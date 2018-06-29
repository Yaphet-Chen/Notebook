
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [Ideal gas law](#ideal-gas-law)
- [Thermodynamics properties](#thermodynamics-properties)
- [Equipartition Theorem](#equipartition-theorem)
- [Entropy](#entropy)
- [Sound speed](#sound-speed)

<!-- /code_chunk_output -->

### Ideal gas law
common forms
$$ PV=NkT=\frac{M}{m}kT=MRT $$

or 
$$ P=\rho RT$$

here:
- P is the pressure of the gas,
- V is the volume of the gas, 
- N is the number of gas molecules (or Avogadro constant times the amount of substance $ N_A n $),
- k is the Boltzmann constant,
- T is the absolute temperature of the gas,
- M is the total mass of the gas,
- m is the molecular mass of the gas,
- $ R=\frac{k}{m} $ is the specific gas constant,
- $ \rho $ is the density of the gas.

### Thermodynamics properties
The **total energy** of gas is (without the consideration of potential energy)
$$ \rho E = \rho e+\frac{1}{2}\rho U^2 $$

where e is the thermal/internal energy of *unit mass* gas, U is the bulk velocity of gas.
The **heat capacity** of an object is the amountof heat needed to raise its temperature by one degree:
$$ C \equiv \frac{\delta Q}{dT} $$

The **specific heat capacity** of a substance is defined as the heat capacity per unit mass:
$$ c \equiv \frac{C}{m} $$

where m is the mass of the object.

By first law of thermodynamics $de = \delta Q - W $, we have
$$ c_v = \frac{\delta Q}{dT} = \frac{de}{dT} $$

where $ c_v $ is the **specific heat capacity at constant volume**.
or
$$ de = c_v dT $$


For isobaric process (*unit mass* here),
$$ c_p dT = \delta Q = de+PdV = de+Pd(\frac{1}{\rho}) = c_vdT+d(\frac{P}{\rho}) = c_vdT+RdT $$

where $ c_p $ is the **specific heat capacity at constant pressure**.
Therefore, we have
$$ c_v+R=c_p $$

The **specific enthalpy** of the gas is 
$$ h=e+\frac{P}{\rho} $$

and
$$ dh = d(e+\frac{P}{\rho}) = c_pdT $$

for isobaric process.

### Equipartition Theorem
The original idea of equipartition was that, in ==*thermal equilibrium*==, energy is shared equally among all of its various forms. For *unit mass* gas, internal energy = translational energy + rotational energy + vibrational energy (T<1600K, no vibration) + $\cdots$.
$$ e = \frac{\alpha}{2}NkT = \frac{\alpha}{2}\frac{k}{m}T = \frac{\alpha}{2}RT $$

where $ \alpha $ is the total number of degree of freedom for each molecule.
Therefore the **specific heat ratio** is
$$ \gamma = \frac{c_p}{c_v} = \frac{\tfrac{\alpha}{2}}{1+\tfrac{\alpha}{2}} = \frac{\alpha+2}{\alpha} $$

- monatomic gas: $ \alpha=3,\gamma=\frac{5}{3} $
- diatomic gas: $ \alpha=5, \gamma=\frac{7}{5}=1.4 $

and
$$ \alpha = \frac{2}{\gamma-1}$$

$$ e = c_vT = \frac{c_v P}{R \rho} = \frac{P}{(\gamma-1)\rho} $$

Thus, the total energy of gas can be rewritten as
$$ \rho E = \rho e+\frac{1}{2}\rho U^2 = \frac{P}{\gamma-1}+\frac{1}{2}\rho U^2, \quad \gamma\in [1,3]. $$

### Entropy
Entropy S(U,V,N) is a function of U, V and N, the change of S can be expressed as
$$ dS = \left(\frac{\partial S}{\partial U}\right)_{V,N}dU + \left(\frac{\partial S}{\partial V}\right)_{U,N}dV + \left(\frac{\partial S}{\partial N}\right)_{U,V}dN $$

and
$$ \frac{1}{T} = \left(\frac{\partial S}{\partial U}\right)_{V,N}, \quad 
    \frac{P}{T}=\left(\frac{\partial S}{\partial V}\right)_{U,N}, \quad
    -\frac{\mu}{T}=\left(\frac{\partial S}{\partial N}\right)_{U,V} $$

where $ \mu $ is the chemical potential.
If U, V and N all change by very small amounts, the resulting change in the entropy function S(U,V,N) is
$$ dS = \frac{1}{T}dU+\frac{P}{T}dV-\frac{\mu}{T}dN $$

Thus, we have **Thermodynamic Identity** for diffusive systems, which is true only for ==*quasi-static process*== such that each step of change is *infinitesimal*. 
$$ dU = TdS-PdV+\sum_i \mu_i dN_i $$

The extra term $ \mu dN $ is sometimes called "**chemical work**".
For *reversible* (at least it should be *quasi-static*) *process*,
$$ W=-PdV, \quad Q=TdS $$

The thermodynamic identity will be equivalent to the first law of thermodynamics.
The general relation between entropy changes and heat transfers (*second law of thermodynamics*) is
$$ dS \geq \frac{\delta Q}{T} \quad or \quad \delta Q \leq TdS $$

Equality holds only for reversible process.
>Isentropic Process ($ \Delta S = 0 $) = adiabatic process (no heat exchange $\delta Q = 0 $) + reversible process.

For ideal gas,
$$ \frac{1}{T}de+\frac{P}{T}d\left(\frac{1}{\rho}\right) = dS \implies c_vlnT-Rln\rho \propto S $$

Therefore,
$$ S \propto ln\frac{T^{c_v}}{\rho^R} \propto ln\frac{P^{c_v}}{\rho^{c_v+R}} \propto ln\frac{P^{c_v}}{\rho^{\gamma c_v}} \propto c_vln\frac{P}{\rho^\gamma} $$

or
$$ S = c_vln\frac{P}{\rho^\gamma}+const $$

Since entropy is a relative quantity, we can define entropy for ideal gas as
$$ S = c_vln\frac{P}{\rho^\gamma} $$

We have
$$ P = e^{\frac{S}{c_v}}\rho^\gamma $$

For isentropic flow, if $ \gamma = 1 \implies \alpha = +\infty $, we have $ P \propto \rho \implies T = const $, which means the gas is in isothermal process. 

### Sound speed
The speed of sound is given by
$$ c = \sqrt{\left(\frac{\partial P}{\partial \rho}\right)_S} =  \sqrt{\frac{\partial \rho^\gamma}{\partial \rho}} = \sqrt{\gamma\rho^{\gamma-1}} = \sqrt{\frac{\gamma \rho^\gamma}{\rho}} = \sqrt{\frac{\gamma P}{\rho}} = \sqrt{\gamma RT} $$

The speed of sound in an ideal gas depends only on its temperature and composition. 
However, in a **dispersive** medium, the speed of sound is a function of sound frequency, through the dispersion relation. Each frequency component propagates at its own speed, called the **phase velocity**, while the energy of the disturbance propagates at the **group velocity**. The same phenomenon occurs with light waves; see optical dispersion for a description.
