
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

* [分子平均自由程](#分子平均自由程)
* [一些重要的数据](#一些重要的数据)
	* [流动的领域划分](#流动的领域划分)
	* [Classification of Mach regimes](#classification-of-mach-regimes)
		* [Dissociated gas](#dissociated-gas)
		* [Ionized gas](#ionized-gas)
		* [Radiation-dominated regime](#radiation-dominated-regime)
	* [几个重要的特征温度](#几个重要的特征温度)
		* [转动与振动](#转动与振动)
		* [离解与电离](#离解与电离)
* [非平衡现象与稀薄气体动力学](#非平衡现象与稀薄气体动力学)
* [相似准则](#相似准则)

<!-- /code_chunk_output -->

# 分子平均自由程

**碰撞频率**$\nu$为单位时间内发生的碰撞次数，等于单位时间内扫过的体积乘以场分子的数密度
$$ \nu = \overline{c_r\sigma_T}n $$

其中$c_r$为分子间相对速度，$\sigma_T$为总碰撞截面。

**平均自由程**$\lambda$为一个分子在两次碰撞间走过距离的平均值，
$$ \lambda = \frac{\bar{c}}{\nu} = \frac{\bar{c}}{\overline{c_r\sigma_T}n} = \frac{\bar{c}m}{\overline{c_r\sigma_T}\rho} $$

其中$\bar{c}$为分子平均热运动速度（平衡态时$ \bar{c} = \sqrt{\frac{8kT}{\pi m}} $），m为分子质量。且由此可知在气体中$ \lambda \rho = const $，或分子的平均自由程与气体密度成反比。

同理，我们有**平均碰撞时间**$ \tau = {}^{\lambda}\!/_{\bar{c}} $。

# 一些重要的数据

**Loschmidt's number** $n_0$ is the number of particles (atoms or molecules) of an ideal gas in a given volume (the number density). It value was 2.686 7774(47)×10^25^ per cubic metre at 0 °C and 1 atm.

高空大气密度随高程降低，分子平均自由程由海平面约 0.07×10^-6^m 增加到 70km 的约 1mm 和 85km 的约 1cm，这时稀薄气体效应显著起来。

## 流动的领域划分

| 流域       | Knudsen数   | 特性                                                                                             |
| :--------: | :---------: | :----------------------------------------------------------------------------------------------: |
| 滑流领域   | 0.01<Kn<0.1 | 边界附近，出现速度在边界的滑移和温度跳跃。                                                       |
| 过渡领域   | 0.1<Kn<10   | 分子与表面的碰撞和来流中分子的互相碰撞有着同等的重要性。                                         |
| 自由分子流 | Kn>10       | 由物体反射的分子只有在飞离物体很远以后才与其他分子碰撞，分子来流的速度分布函数不受物体存在影响。 |

>在高超声速绕流问题中，由于冷壁的存在，从物体表面散射的分子与来流分子相碰撞的平均自由程$\lambda_i$要比$\lambda$小得多，因此流动满足自由分子流的要求要比上述分流要严格一些。

## Classification of Mach regimes

| Regime          | Mach number |
| :-------------: | :---------: |
| Subsonic        | <0.8        |
| Transonic       | 0.8–1.2     |
| Supersonic      | 1.2–5.0     |
| Hypersonic      | 5.0–10.0    |
| High-hypersonic | 10.0–25.0   |
| Re-entry speeds | >25.0       |

High temperatures due to a manifestation of viscous dissipation cause non-equilibrium chemical flow properties such as ***vibrational excitation*** and ***dissociation*** and ***ionization*** of molecules resulting in *convective* and *radiative heat-flux*. These effects collectively become important around `Mach 5`.

### Dissociated gas

The type of surface material also has an effect on the flow because it serves as ***surface catalysis***. The lower border of this regime is where any component of a gas mixture first begins to dissociate in the stagnation point of a flow (which for nitrogen is around `2000 K`). At the upper border of this regime, the effects of ionization start to have an effect on the flow.

### Ionized gas

In this regime the ionized electron population of the stagnated flow becomes significant, and the electrons must be modeled separately. Often the electron temperature is handled separately from the temperature of the remaining gas components. This region occurs for freestream flow velocities around `10–12 km/s`. Gases in this region are modeled as ***non-radiating plasmas***.

### Radiation-dominated regime

Above around `12 km/s`, the heat transfer to a vehicle changes from being conductively dominated to radiatively dominated. The modeling of gases in this regime is split into two classes: *Optically thin* and *Optically thick*.

*[Optically thin]: where the gas does not re-absorb radiation emitted from other parts of the gas.
*[Optically thick]: where the radiation must be considered a separate source of energy.

## 几个重要的特征温度

航天飞行器穿过高空大气的速度约在$ U=7km/s $到$ 10km/s $之间。在驻点，气体的这样高的动能要转换为内能。用理想气体的能量守恒关系式推出的驻点温度$ T_0 $为
$$ T_0 = T+\frac{U^2}{2c_p} = T\left(1+\frac{U^2}{2 c_p T}\right) = T\left(1+\frac{\gamma-1}{2}M^2\right) $$

取比热比$ \gamma=1.4 $，来流静温$ T=300K $，可得

* $ U=7km/s \implies M=20 $时，$ T_0=24700K $。
* $ U=10km/s \implies M=30 $时，$ T_0=50100K $。

但实际上驻点温度远没有这样高，这是因为能量用来==激发气体分子的内自由度==和被气体中==离解过程的吸热反应==吸收了的缘故。

>空气是由76.3%（摩尔比）的N~2~和23.7%的O~2~组成的混合气体。在较高温度下，气体内部能态产生变化，空气会离解为O和N，并有NO产生，在更高的温度下发生电离，产生相应的离子和电子（并有辐射发生）。

### 转动与振动

我们将相应的能量值除以$k$分别得到
**转动特征温度**$ \Theta_r $
$$ \Theta_r=h^2/(8\pi^2Ik) $$

**振动特征温度**$ \Theta_v $
$$ \Theta_v=h\nu/k $$

式中，$h$为Planck常数；$k$为Boltzmann常数；$I$为分子转动惯量；$\nu$为振动频率。
对于空气中的N~2~，NO和O~2~，转动特征温度只有几K，其转动特征温度分别为
$$ \Theta_r=2.88K,2.44K,2.07K $$

正是因为氮和氧分子有这样低的转动特征温度，所以在室温下，转动能就充分激发起来。
而相应的N~2~，NO和O~2~振动特征温度为
$$ \Theta_v=3371K,2719K,2256K$$

由于振动特征温度有较高的值，振动能在较高的温度下才被激发起来，高温下气体能量的一部分要用来激发振动能。

### 离解与电离

空气中发生的吸热离解反应进一步解释高超声速气流中驻点温度达不到预期值的原因。
**离解特征温度**$ \Theta_d $为离解能除以$k$。其中O~2~，NO，N~2~的离解特征温度为
$$ \Theta_d = 59500K,75500K,113500K $$

在考虑驻点区的离解，看来$T$比$\Theta_d$显得要小得多。这时仍有显著离解的原因有两个。

* 碰撞中高能量的粒子碰撞的机会要多。
* *复合反应是放热反应*，需要有第三体的参与将能量带走才可能发生，而三体碰撞的几率是很小的，使离解占主导地位。而较高的离解特征温度(对应的离解能也较高)还使离解反应降低温度的作用变得显著。

当温度达到更高时，电离反应开始发生并变得重要。其中O~2~，NO，N~2~的**电离特征温度**$ \Theta_i $为
$$ \Theta_i = 142000K,108000K,181000K $$

大约温度要达到`10000K`时，电离才显现自己的作用。

# 非平衡现象与稀薄气体动力学

>稀薄气体动力学=分子动理论+分子内部结构变化（内能激发、离解（化学反应）、电离（电子能级激发、辐射））

气体分子的内态激发、化学反应等都是**速率过程**，完成一个过程需要一定的时间，以松弛时间$\tau$来度量。由于这些过程都是在分子的碰撞中完成的，松弛时间正比于分子的平均碰撞时间$\tau$，松弛完成的距离正比于分子的平均自由程$\lambda$。
*转动松弛时间*通常大约为5～10个平均碰撞时间，*振动松弛*在正常温度下蛋比平动和转动松弛慢两、三个量级。
当松弛时间和松弛距离与流动特征时间和流场特征距离相比为较大时，内能和化学反应的非平衡出现。**非平衡现象**总是当流动条件向稀薄气体流动变化时变得更为严重，而高速稀薄气流中的内能和化学过程通常是处于非平衡态。

# 相似准则

由于在VSS模型中，我们可以得到平衡态的平均自由程
$$ \lambda_0=\frac{4\alpha(7-2\omega)(5-2\omega)}{5(\alpha+1)(\alpha+2)}\left(\frac{m}{2\pi kT}\right)^{1/2}\frac{\mu}{\rho} = \frac{4\alpha(7-2\omega)(5-2\omega)}{5(\alpha+1)(\alpha+2)} \sqrt{\frac{\gamma}{2\pi}} \frac{\mu}{a\rho}$$

由此容易得到下面的基本关系式
$$ Kn=\frac{\lambda}{L} = \frac{4\alpha(7-2\omega)(5-2\omega)}{5(\alpha+1)(\alpha+2)} \sqrt{\frac{\gamma}{2\pi}} \frac{M}{Re}$$

式中$ Re=\rho UL/\mu $中的特征长度与$Kn$相同。这样，两种流动稀薄程度的相似，要求 $M/Re$ 比值不变。对于不太高速的流动，两种流动相似要求$Ma$数和$Re$数相同，也就有$Kn$数相同。由上式，流动相似要求$Ma$，$Re$和$Kn$三个参数中任意两个相同。

>当讨论的问题的特征尺度十分细小时，如在讨论MEMS（纳米抗电系统）问题时，不能只考虑$Kn$数的模拟，==真实分子数相同是关键，流场量的涨落是真实的==。由于宏观量的方差与粒子数的平方根$\sqrt{N}$成反比，当特征体积中分子的真实数目小到一定程度，会引起宏观量的涨落问题。

>对于航天领域的高速流动而言，仅有$Kn$数和$Ma$数的相似是不够的。高速的或者有时称为高焓的反应流动的相似准则是**双尺度律/双体碰撞模拟律(binary scaling law)**，即两种流动的静温相同，且
$$ U_\infty,\rho_\infty L $$
>
>相同时为相似。