# Satellite-Orbit-Simulation

This program simulates a satellite's Low Earth Orbit (LEO) trajectory and additionally outputs its Ground Track based on a custom launch position and speed.

## Orbit Analyzer

The program performs several operations, including the conversion of **State Vectors** (which describe the position and velocity of the satellite) into **Kepler's Orbital Elements**. This process involves the following:

1. **Position Vector** \([R_x, R_y, R_z]\): The position of the satellite in 3D space.
2. **Velocity Vector** \([V_x, V_y, V_z]\): The velocity of the satellite in the same 3D coordinates.

After converting these vectors, the program computes the following **Kepler's Orbital Elements**:

1. **Semi-major axis (a)**: The length of the orbit's major axis, which determines the orbit's size.
2. **Eccentricity (e)**: A measure of how elliptical the orbit is (as opposed to circular).
3. **Inclination (inc)**: The tilt of the orbit with respect to Earth's equator.
4. **Right Ascension of Ascending Node (RAAN)**: The angle that measures the position of the ascending node of the orbit.
5. **Argument of Perigee (ω)**: The position of the orbit where the satellite is closest to Earth.
6. **Initial Mean Anomaly (M₀)**: The angle that determines the position of the satellite along its orbit at the initial time.

## Orbit Visualization

After the orbital elements are computed, the program visualizes the satellite's trajectory in **3D**. The visualization includes:

- **Blue Sphere**: Represents the Earth.
- **Green Sphere**: Shows the satellite's initial position.
- **Red Spheres**: Show the satellite's position at fixed time intervals during the simulation.
- **Dotted Green Line**: Represents the satellite's initial velocity vector.
- **Three Orthogonal Black Lines**: Represent the positive axes of the Earth Centered Inertial (ECI) coordinate system.

## Simulation Results

At the end of the simulation, the program outputs:

- **Altitude ranges**: The altitude of the satellite throughout the orbit.
- **Orbit Type**: Either **LEO (Low Earth Orbit)** or **MEO (Medium Earth Orbit)**.

The simulation only takes into account the influence of **Earth's gravity** and does not consider other forces like atmospheric drag or the influence of other satellites or planets.

## Authors

Piazza Edoardo, Uboldi Francesca, Cuorici Melania
