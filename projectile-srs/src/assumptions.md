# Assumptions

This section simplifies the original problem and helps in developing the theoretical models by filling in the missing information for the physical system. The assumptions refine the scope by providing more detail.

twoDMotion: The projectile motion is two-dimensional (2D). (RefBy: [GD:velVec]() and [GD:posVec]().)

cartSyst: A Cartesian coordinate system is used (from [A:neglectCurv]()). (RefBy: [GD:velVec]() and [GD:posVec]().)

yAxisGravity: The direction of the y-axis is directed opposite to gravity. (RefBy: [IM:calOfLandingDist](), [IM:calOfLandingTime](), and [A:accelYGravity]().)

launchOrigin: The launcher is coincident with the origin. (RefBy: [IM:calOfLandingDist]() and [IM:calOfLandingTime]().)

targetXAxis: The target lies on the x-axis (from [A:neglectCurv]()). (RefBy: [IM:calOfLandingTime]().)

posXDirection: The positive x-direction is from the launcher to the target. (RefBy: [IM:offsetIM](), [IM:messageIM](), [IM:calOfLandingDist](), and [IM:calOfLandingTime]().)

constAccel: The acceleration is constant (from [A:accelXZero](), [A:accelYGravity](), [A:neglectDrag](), and [A:freeFlight]()). (RefBy: [GD:velVec]() and [GD:posVec]().)

accelXZero: The acceleration in the x-direction is zero. (RefBy: [IM:calOfLandingDist]() and [A:constAccel]().)

accelYGravity: The acceleration in the y-direction is the acceleration due to gravity (from [A:yAxisGravity]()). (RefBy: [IM:calOfLandingTime]() and [A:constAccel]().)

neglectDrag: Air drag is neglected. (RefBy: [A:constAccel]().)

pointMass: The size and shape of the projectile are negligible, so that it can be modelled as a point mass. (RefBy: [GD:rectVel]() and [GD:rectPos]().)

freeFlight: The flight is free; there are no collisions during the trajectory of the projectile. (RefBy: [A:constAccel]().)

neglectCurv: The distance is small enough that the curvature of the celestial body can be neglected. (RefBy: [A:targetXAxis]() and [A:cartSyst]().)

timeStartZero: Time starts at zero. (RefBy: [GD:velVec](), [GD:rectVel](), [GD:rectPos](), [GD:posVec](), and [IM:calOfLandingTime]().)

gravAccelValue: The acceleration due to gravity is assumed to have the value provided in the section for Values of Auxiliary Constants. (RefBy: [IM:calOfLandingDist]() and [IM:calOfLandingTime]().)
