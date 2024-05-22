# Traceability Matrices and Graphs

The purpose of the traceability matrices is to provide easy references on what has to be additionally modified if a certain component is changed. Every time a component is changed, the items in the column of that component that are marked with an "X" should be modified as well. [Tab:TraceMatAvsA]() shows the dependencies of the assumptions on each other. [Tab:TraceMatAvsAll]() shows the dependencies of the data definitions, theoretical models, general definitions, instance models, requirements, likely changes, and unlikely changes on the assumptions. [Tab:TraceMatRefvsRef]() shows the dependencies of the data definitions, theoretical models, general definitions, and instance models on each other. [Tab:TraceMatAllvsR]() shows the dependencies of the requirements and goal statements on the data definitions, theoretical models, general definitions, and instance models.

||[A:twoDMotion]()|[A:cartSyst]()|[A:yAxisGravity]()|[A:launchOrigin]()|[A:targetXAxis]()|[A:posXDirection]()|[A:constAccel]()|[A:accelXZero]()|[A:accelYGravity]()|[A:neglectDrag]()|[A:pointMass]()|[A:freeFlight]()|[A:neglectCurv]()|[A:timeStartZero]()|[A:gravAccelValue]()|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|[A:twoDMotion]()||||||||||||||||
|[A:cartSyst]()|||||||||||||X|||
|[A:yAxisGravity]()||||||||||||||||
|[A:launchOrigin]()||||||||||||||||
|[A:targetXAxis]()|||||||||||||X|||
|[A:posXDirection]()||||||||||||||||
|[A:constAccel]()||||||||X|X|X||X||||
|[A:accelXZero]()||||||||||||||||
|[A:accelYGravity]()|||X|||||||||||||
|[A:neglectDrag]()||||||||||||||||
|[A:pointMass]()||||||||||||||||
|[A:freeFlight]()||||||||||||||||
|[A:neglectCurv]()||||||||||||||||
|[A:timeStartZero]()||||||||||||||||
|[A:gravAccelValue]()||||||||||||||||

**<p align="center">Traceability Matrix Showing the Connections Between Assumptions and Other Assumptions</p>**

</br>

||[DD:vecMag]()|[DD:speedIX]()|[DD:speedIY]()|[TM:acceleration]()|[TM:velocity]()|[GD:rectVel]()|[GD:rectPos]()|[GD:velVec]()|[GD:posVec]()|[IM:calOfLandingTime]()|[IM:calOfLandingDist]()|[IM:offsetIM]()|[IM:messageIM]()|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|[DD:vecMag]()||||||||||||||
|[DD:speedIX]()|X|||||||||||||
|[DD:speedIY]()||X||||||||||||
|[TM:acceleration]()||||||||||||||
|[TM:velocity]()||||||||||||||
|[GD:rectVel]()||||X||||||||||
|[GD:rectPos]()|||||X|X||||||||
|[GD:velVec]()|||||||X|||||||
|[GD:posVec]()|||||||X|||||||
|[IM:calOfLandingTime]()|||X||||||X|||||
|[IM:calOfLandingDist]()||X|||||||X|X||||
|[IM:offsetIM]()|||||||||||X|||
|[IM:messageIM]()||||||||||||X||

**<p align="center">Traceability Matrix Showing the Connections Between Items and Other Sections</p>**

</br>

||[DD:vecMag]()|[DD:speedIX]()|[DD:speedIY]()|[TM:acceleration]()|[TM:velocity]()|[GD:rectVel]()|[GD:rectPos]()|[GD:velVec]()|[GD:posVec]()|[IM:calOfLandingTime]()|[IM:calOfLandingDist]()|[IM:offsetIM]()|[IM:messageIM]()|[FR:Input-Values]()|[FR:Verify-Input-Values]()|[FR:Calculate-Values]()|[FR:Output-Values]()|[NFR:Correct]()|[NFR:Verifiable]()|[NFR:Understandable]()|[NFR:Reusable]()|[NFR:Maintainable]()|[NFR:Portable]()|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|[GS:targetHit]()||||||||||||||||||||||||
|[FR:Input-Values]()||||||||||||||||||||||||
|[FR:Verify-Input-Values]()||||||||||||||||||||||||
|[FR:Calculate-Values]()|||||||||||X|X|X|X||||||||||
|[FR:Output-Values]()|||||||||||X||X|X||||||||||
|[NFR:Correct]()||||||||||||||||||||||||
|[NFR:Verifiable]()||||||||||||||||||||||||
|[NFR:Understandable]()||||||||||||||||||||||||
|[NFR:Reusable]()||||||||||||||||||||||||
|[NFR:Maintainable]()||||||||||||||||||||||||
|[NFR:Portable]()||||||||||||||||||||||||

**<p align="center">Traceability Matrix Showing the Connections Between Requirements, Goal Statements and Other Items</p>**

The purpose of the traceability graphs is also to provide easy references on what has to be additionally modified if a certain component is changed. The arrows in the graphs represent dependencies. The component at the tail of an arrow is depended on by the component at the head of that arrow. Therefore, if a component is changed, the components that it points to should also be changed. [Fig:TraceGraphAvsA]() shows the dependencies of assumptions on each other. [Fig:TraceGraphAvsAll]() shows the dependencies of data definitions, theoretical models, general definitions, instance models, requirements, likely changes, and unlikely changes on the assumptions. [Fig:TraceGraphRefvsRef]() shows the dependencies of data definitions, theoretical models, general definitions, and instance models on each other. [Fig:TraceGraphAllvsR]() shows the dependencies of requirements and goal statements on the data definitions, theoretical models, general definitions, and instance models. [Fig:TraceGraphAllvsAll]() shows the dependencies of dependencies of assumptions, models, definitions, requirements, goals, and changes with each other.

![TraceGraphAvsA](./traceygraphs/avsa.svg)

**<p align="center">TraceGraphAvsA</p>**

![TraceGraphAvsAll](./traceygraphs/avsall.svg)

**<p align="center">TraceGraphAvsAll</p>**

![TraceGraphRefvsRef](./traceygraphs/refvsref.svg)

**<p align="center">TraceGraphRefvsRef</p>**

![TraceGraphAllvsR](./traceygraphs/allvsr.svg)

**<p align="center">TraceGraphAllvsR</p>**

![TraceGraphAllvsAll](./traceygraphs/allvsall.svg)

**<p align="center">TraceGraphAllvsAll</p>**

For convenience, the following graphs can be found at the links below:

- [TraceGraphAvsA](./traceygraphs/avsa.svg)
- [TraceGraphAvsAll](./traceygraphs/avsall.svg)
- [TraceGraphRefvsRef](./traceygraphs/refvsref.svg)
- [TraceGraphAllvsR](./traceygraphs/allvsr.svg)
- [TraceGraphAllvsAll](./traceygraphs/allvsall.svg)
