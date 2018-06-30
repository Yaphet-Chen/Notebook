
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [Classification of Mach regimes](#classification-of-mach-regimes)
        - [Dissociated gas](#dissociated-gas)
        - [Ionized gas](#ionized-gas)
        - [Radiation-dominated regime](#radiation-dominated-regime)
- [Some interesting data](#some-interesting-data)
- [平均自由程](#%E5%B9%B3%E5%9D%87%E8%87%AA%E7%94%B1%E7%A8%8B)
- [流动的领域划分](#%E6%B5%81%E5%8A%A8%E7%9A%84%E9%A2%86%E5%9F%9F%E5%88%92%E5%88%86)

<!-- /code_chunk_output -->

>稀薄气体动力学=分子动理论+分子内部结构变化（内能激发、化学反应、电子能级激发）

# Classification of Mach regimes

| Regime          | Mach number |
| :-------------: | :---------: |
| Subsonic        | <0.8        |
| Transonic       | 0.8–1.2     |
| Supersonic      | 1.2–5.0     |
| Hypersonic      | 5.0–10.0    |
| High-hypersonic | 10.0–25.0   |
| Re-entry speeds | >25.0       |

High temperatures due to a manifestation of viscous dissipation cause non-equilibrium chemical flow properties such as ***vibrational excitation*** and ***dissociation*** and ***ionization*** of molecules resulting in *convective* and *radiative heat-flux*. These effects collectively become important around `Mach 5`.

## Dissociated gas

The type of surface material also has an effect on the flow because it serves as ***surface catalysis***. The lower border of this regime is where any component of a gas mixture first begins to dissociate in the stagnation point of a flow (which for nitrogen is around `2000 K`). At the upper border of this regime, the effects of ionization start to have an effect on the flow.

## Ionized gas

In this regime the ionized electron population of the stagnated flow becomes significant, and the electrons must be modeled separately. Often the electron temperature is handled separately from the temperature of the remaining gas components. This region occurs for freestream flow velocities around `10–12 km/s`. Gases in this region are modeled as ***non-radiating plasmas***.

## Radiation-dominated regime

Above around `12 km/s`, the heat transfer to a vehicle changes from being conductively dominated to radiatively dominated. The modeling of gases in this regime is split into two classes: *Optically thin* and *Optically thick*.

*[Optically thin]: where the gas does not re-absorb radiation emitted from other parts of the gas.
*[Optically thick]: where the radiation must be considered a separate source of energy.

# Some interesting data

**Loschmidt's number** $n_0$ is the number of particles (atoms or molecules) of an ideal gas in a given volume (the number density). It value was 2.686 7774(47)×10^25^ per cubic metre at 0 °C and 1 atm.

高空大气密度随高程降低，分子平均自由程由海平面约 0.07×10^-6^m 增加到 70km 的约 1mm 和 85km 的约 1cm，这时稀薄气体效应显著起来。

# 平均自由程

**碰撞频率**$\nu$为单位时间内发生的碰撞次数，等于单位时间内扫过的体积乘以场分子的数密度
$$ \nu = \overline{c_r\sigma_T}n $$

其中$c_r$为分子间相对速度，$\sigma_T$为总碰撞截面。
**平均自由程**$\lambda$为一个分子在两次碰撞间走过距离的平均值，
$$ \lambda = \frac{\bar{c}}{\nu} = \frac{\bar{c}}{\overline{c_r\sigma_T}n} = \frac{\bar{c}m}{\overline{c_r\sigma_T}\rho} $$

其中$\bar{c}$为分子的平均热运动速度，m为分子质量。且由此可知在气体中$ \lambda \rho = const $，或分子的平均自由程与气体密度成反比。

# 流动的领域划分

| 流域       | Knudsen数   | 特性                                                                                             |
| :--------: | :---------: | :----------------------------------------------------------------------------------------------: |
| 滑流领域   | 0.01<Kn<0.1 | 边界附近，出现速度在边界的滑移和温度跳跃。                                                       |
| 过渡领域   | 0.1<Kn<10   | 分子与表面的碰撞和来流中分子的互相碰撞有着同等的重要性。                                         |
| 自由分子流 | Kn>10       | 由物体反射的分子只有在飞离物体很远以后才与其他分子碰撞，分子来流的速度分布函数不受物体存在影响。 |

>在高超声速绕流问题中，由于冷壁的存在，从物体表面散射的分子与来流分子相碰撞的平均自由程$\lambda_i$要比$\lambda$小得多，因此流动满足自由分子流的要求要比上述分流要严格一些。