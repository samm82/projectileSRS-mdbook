# Instance Models

This section transforms the problem defined in the [problem description](./problem-description.md) into one which is expressed in mathematical terms. It uses concrete symbols defined in the [data definitions](./data-definitions.md) to replace the abstract symbols in the models identified in [theoretical models](./theoretical-models.md) and [general definitions](./general-definitions.md).

|Refname|IM:calOfLandingTime|
|-|-|
|Label|Calculation of landing time|
|Input|\\({v_{\text{launch}}}\\), \\(θ\\)|
|Output|\\({t_{\text{flight}}}\\)|
|Input Constraints|\\[{v_{\text{launch}}}\gt{}0\\] \\[0\lt{}θ\lt{}\frac{π}{2}\\]|
|Output Constraints|\\[{t_{\text{flight}}}\gt{}0\\]|
|Equation|\\[{t_{\text{flight}}}=\frac{2 {v_{\text{launch}}} \sin\left(θ\right)}{g}\\]|
|Description|<ul><li> \\({t_{\text{flight}}}\\) is the flight duration (\\({\text{s}}\\)) </li><li> \\({v_{\text{launch}}}\\) is the launch speed (\\(\frac{\text{m}}{\text{s}}\\)) </li><li> \\(θ\\) is the launch angle (\\({\text{rad}}\\)) </li><li> \\(g\\) is the magnitude of gravitational acceleration (\\(\frac{\text{m}}{\text{s}^{2}}\\)) </li></ul>|
|Notes|<ul><li> The constraint \\(0\lt{}θ\lt{}\frac{π}{2}\\) is from [A:posXDirection]() and [A:yAxisGravity](), and is shown in [Fig:Launch](). </li><li> \\(g\\) is defined in [A:gravAccelValue](). </li><li> The constraint \\({t_{\text{flight}}}\gt{}0\\) is from [A:timeStartZero](). </li></ul>|
|Source|--|
|RefBy|[IM:calOfLandingDist](), [FR:Output-Values](), and [FR:Calculate-Values]()|

#### Detailed derivation of flight duration:

We know that \\({{p_{\text{y}}}^{\text{i}}}=0\\) ([A:launchOrigin]()) and \\({{a_{\text{y}}}^{\text{c}}}=-g\\) ([A:accelYGravity]()). Substituting these values into the y-direction of [GD:posVec]() gives us:

\\[{p_{\text{y}}}={{v_{\text{y}}}^{\text{i}}} t-\frac{g t^{2}}{2}\\]

To find the time that the projectile lands, we want to find the \\(t\\) value (\\({t_{\text{flight}}}\\)) where \\({p_{\text{y}}}=0\\) (since the target is on the \\(x\\)-axis from [targetXAxis]()). From the equation above we get:

\\[{{v_{\text{y}}}^{\text{i}}} {t_{\text{flight}}}-\frac{g {t_{\text{flight}}}^{2}}{2}=0\\]

Dividing by \\({t_{\text{flight}}}\\) (with the constraint \\({t_{\text{flight}}}\gt{}0\\)) gives us:

\\[{{v_{\text{y}}}^{\text{i}}}-\frac{g {t_{\text{flight}}}}{2}=0\\]

Solving for \\({t_{\text{flight}}}\\) gives us:

\\[{t_{\text{flight}}}=\frac{2 {{v_{\text{y}}}^{\text{i}}}}{g}\\]

From [DD:speedIY]() (with \\({v^{\text{i}}}={v_{\text{launch}}}\\)) we can replace \\({{v_{\text{y}}}^{\text{i}}}\\):

\\[{t_{\text{flight}}}=\frac{2 {v_{\text{launch}}} \sin\left(θ\right)}{g}\\]

|Refname|IM:calOfLandingDist|
|-|-|
|Label|Calculation of landing position|
|Input||
|Output||
|Input Constraints||
|Output Constraints||
|Equation||
|Description|<ul><li>  </li><li>  </li><li>  </li><li>  </li></ul>|
|Notes|<ul><li>  </li><li>  </li><li>  </li></ul>|
|Source|--|
|RefBy|[IM:offsetIM]() and [FR:Calculate-Values]()|

|Refname|IM:offsetIM|
|-|-|
|Label|Offset|
|Input||
|Output||
|Input Constraints||
|Output Constraints| |
|Equation||
|Description|<ul><li>  </li><li>  </li><li>  </li></ul>|
|Notes|<ul><li>  </li><li>  </li></ul>|
|Source|--|
|RefBy|[IM:messageIM](), [FR:Output-Values](), and [FR:Calculate-Values]()|

|Refname|IM:messageIM|
|-|-|
|Label|Output message|
|Input||
|Output||
|Input Constraints||
|Output Constraints||
|Equation||
|Description|<ul><li>  </li><li>  </li><li>  </li><li>  </li></ul>|
|Notes|<ul><li>  </li><li>  </li><li>  </li><li>  </li></ul>|
|Source|--|
|RefBy|[FR:Output-Values]() and [FR:Calculate-Values]()|

