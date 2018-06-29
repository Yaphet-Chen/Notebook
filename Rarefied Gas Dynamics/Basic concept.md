
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [Classification of Mach regimes](#classification-of-mach-regimes)
                - [Dissociated gas](#dissociated-gas)
                - [Ionized gas](#ionized-gas)
                - [Radiation-dominated regime](#radiation-dominated-regime)
- [Some interesting datakv](#some-interesting-datakv)

<!-- /code_chunk_output -->

>稀薄气体动力学=分子动理论+分子内部结构变化（内能激发、化学反应、电子能级激发）

### Classification of Mach regimes
| Regime          | Mach number |
| :-------------: | :---------: |
| Subsonic        | <0.8        |
| Transonic       | 0.8–1.2     |
| Supersonic      | 1.2–5.0     |
| Hypersonic      | 5.0–10.0    |
| High-hypersonic | 10.0–25.0   |
| Re-entry speeds | >25.0       |

High temperatures due to a manifestation of viscous dissipation cause non-equilibrium chemical flow properties such as ***vibrational excitation*** and ***dissociation*** and ***ionization*** of molecules resulting in *convective* and *radiative heat-flux*. These effects collectively become important around `Mach 5`.

##### Dissociated gas 
The type of surface material also has an effect on the flow because it serves as ***surface catalysis***. The lower border of this regime is where any component of a gas mixture first begins to dissociate in the stagnation point of a flow (which for nitrogen is around `2000 K`). At the upper border of this regime, the effects of ionization start to have an effect on the flow.

##### Ionized gas
In this regime the ionized electron population of the stagnated flow becomes significant, and the electrons must be modeled separately. Often the electron temperature is handled separately from the temperature of the remaining gas components. This region occurs for freestream flow velocities around `10–12 km/s`. Gases in this region are modeled as ***non-radiating plasmas***.

##### Radiation-dominated regime
Above around `12 km/s`, the heat transfer to a vehicle changes from being conductively dominated to radiatively dominated. The modeling of gases in this regime is split into two classes: *Optically thin* and *Optically thick*.

*[Optically thin]: where the gas does not re-absorb radiation emitted from other parts of the gas.
*[Optically thick]: where the radiation must be considered a separate source of energy.

### Some interesting datakv
**Loschmidt's number** $n_0$ is the number of particles (atoms or molecules) of an ideal gas in a given volume (the number density). It value was 2.686 7774(47)×10^25^ per cubic metre at 0 °C and 1 atm.

高空大气密度随高程降低，分子平均自由程由海平面约 0.07×10^-6^m 增加到 70km 的约 1mm 和 85km 的约 1cm，这时稀薄气体效应显著起来。
