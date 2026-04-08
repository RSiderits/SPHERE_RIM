README – Sphere Rim Volume Calculator

PURPOSE
This calculator is designed to estimate the relative volume of protein expression in a tumor when staining is localized primarily to the outer rim. This pattern is commonly observed with markers associated with hypoxia, where expression is enriched at the ischemic tumor margin rather than the central tumor core.

The tool assumes a roughly spherical tumor geometry and calculates the proportion of total tumor volume represented by the outer “rim” of expression. This allows for normalization of rim-based staining relative to overall tumor size, which is critical for meaningful interpretation.

FEATURES
- Calculates total tumor volume (mm³)
- Calculates inner core (non-rim) volume (mm³)
- Calculates rim volume (mm³)
- Calculates rim volume as a percentage of total tumor volume
- Calculates rim thickness (mm)
- Provides a live, scaled diagram of the tumor and expression rim
- Dynamic visualization updates based on user input
- Built-in validation to prevent invalid geometry (e.g., inner radius ≥ outer radius)

HOW IT WORKS
The calculator uses the standard formula for the volume of a sphere:

    Volume = (4/3) × π × r³

Where:
- r = radius of the sphere

Steps:
1. The user inputs:
   - Outer tumor radius (mm)
   - Inner rim radius (mm)

2. The calculator computes:
   - Total tumor volume using the outer radius
   - Inner core volume using the inner radius

3. Rim volume is calculated as:
   Rim Volume = Total Volume − Inner Volume

4. Rim percentage is calculated as:
   Rim % = (Rim Volume / Total Volume) × 100

5. Rim thickness is calculated as:
   Thickness = Outer Radius − Inner Radius

HOW TO USE
1. Enter the outer tumor radius in millimeters.
2. Enter the inner radius representing the boundary between the tumor core and the staining rim.
3. Click “Calculate” (or allow automatic update).
4. Review:
   - Absolute volumes (mm³)
   - Rim thickness (mm)
   - Rim percentage (%)
   - Live diagram visualization

INTERPRETATION
- A larger rim percentage indicates that a greater proportion of the tumor volume is composed of the staining region.
- If the outer radius remains constant and the inner radius decreases, the rim volume proportion increases.
- This provides a way to normalize rim-based staining intensity relative to tumor size, which is especially useful in evaluating hypoxia-related markers.

ASSUMPTIONS
- The tumor is approximately spherical.
- The staining pattern forms a continuous outer shell (rim).
- The inner radius accurately represents the boundary of expression.
- Tissue distortion and irregular morphology are not accounted for.

LIMITATIONS
- Real tumors are not perfectly spherical.
- Heterogeneous or patchy staining patterns are not modeled.
- Does not account for necrosis, stromal variation, or non-uniform expression gradients.

This tool is intended for estimation, standardization, and comparative analysis—not absolute quantification.
