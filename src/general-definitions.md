# General Definitions

This section collects the laws and equations that will be used to build the instance models.

|**Refname**|**GD:rectVel**|
|-|-|
|**Label**|Rectilinear (1D) velocity as a function of time for constant acceleration|
|**Units**|\\(\frac{\text{m}}{\text{s}}\\)|
|**Equation**|\\[v\text{(}t\text{)}={v^{\text{i}}}+{a^{c}} t\\]|
|**Description**|<ul><li>\\(v\text{(}t\text{)}\\) is the 1D speed (\\(\frac{\text{m}}{\text{s}}\\)) </li> <li> \\({v^{\text{i}}}\\) is the initial speed (\\(\frac{\text{m}}{\text{s}}\\)) </li> <li> \\({a^{c}}\\) is the constant acceleration (\\(\frac{\text{m}}{\text{s}^{2}}\\)) </li><li>\\(t\\) is the time (\\({\text{s}}\\)) </li></ul>|
|**Source**|[hibbeler2004]() (pg. 8)|
|**RefBy**|[GD:velVec]() and [GD:rectPos]()|

#### Detailed derivation of rectilinear velocity:

Assume we have rectilinear motion of a particle (of negligible size and shape, from [A:pointMass]()); that is, motion in a straight line. The velocity is \\(v\\) and the acceleration is \\(a\\). The motion in [TM:acceleration]() is now one-dimensional with a constant acceleration, represented by \\({a^{c}}\\). The initial velocity (at \\(t = 0\\), from [A:timeStartZero]()) is represented by \\({v^{\text{i}}}\\). [TM:acceleration]() in 1D, and using the above symbols we have:

\\[{a^{c}}=\frac{\\,dv}{\\,dt}\\]

Rearranging and integrating, we have:

\\[\int_{{v^{\text{i}}}}^{v}\\,{1}\\,dv=\int_{0}^{t}\\,{{a^{c}}}\\,dt\\]

Performing the integration, we have the required equation:

\\[v\text{(}t\text{)}={v^{\text{i}}}+{a^{c}} t\\]
