# Functional Requirements

This section provides the functional requirements, the tasks and behaviours that the software is expected to complete.

Input-Values: Input the values from [Tab:ReqInputs]().

Verify-Input-Values: Check the entered input values to ensure that they do not exceed the [data constraints](./data-constraints.md). If any of the input values are out of bounds, an error message is displayed and the calculations stop.

Calculate-Values: Calculate the following values: \\({t_{\text{flight}}}\\) (from [IM:calOfLandingTime]()), \\({p_{\text{land}}}\\) (from [IM:calOfLandingDist]()), \\({d_{\text{offset}}}\\) (from [IM:offsetIM]()), and \\(s\\) (from [IM:messageIM]()).

Output-Values: Output \\({t_{\text{flight}}}\\) (from [IM:calOfLandingTime]()), \\(s\\) (from [IM:messageIM]()), and \\({d_{\text{offset}}}\\) (from [IM:offsetIM]()).

|Symbol|Description|Units|
|-|-|-|
|\\({p_{\text{target}}}\\)|Target position|\\({\text{m}}\\)|
|\\({v_{\text{launch}}}\\)|Launch speed|\\(\frac{\text{m}}{\text{s}}\\)|
|\\(θ\\)|Launch angle|\\({\text{rad}}\\)|

**<p align="center">Required Inputs following <a href="">FR:Input-Values</a></p>**