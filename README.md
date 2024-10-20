# Electric Lines and Potential Simulation (2D Visualization)
A Python tool that visualizes electric field lines and potential in a 2D space for simple charge distributions like point charges.
<br>
Team - Nidhi V J, Keerthi S, Shreya S, Sneha B S, Swetha G K (Ramaiah Skill Academy)

## Project Overview
This project provides a Python tool to simulate electric fields and potentials generated by simple charge distributions in a two-dimensional space. The simulation visualizes electric lines of force and the scalar electric potential, allowing users to better understand electrostatic concepts.

## Features
- Simulate point charges and uniform charge distributions.
- Visualize electric field lines and equipotential lines.
- Interactive plots to explore electric fields.
- Export plots for presentations or reports.Requirements

## Requirements
- Python
- NumPy
- Matplotlib
  
# Electric Field

The electric field \( \mathbf{E} \) around a charge is a vector field that represents the force per unit charge exerted on a positive test charge placed in the field. It is defined as:

\[
\mathbf{E} = \frac{\mathbf{F}}{q}
\]

Where \( \mathbf{F} \) is the force experienced by the test charge \( q \).

For a point charge \( Q \), the electric field at a distance \( r \) is given by:

\[
\mathbf{E} = k \cdot \frac{|Q|}{r^2}
\]

Where \( k \) is Coulomb's constant \( (8.99 \times 10^9 \, \text{Nm}^2/\text{C}^2) \).

# Electric Potential

The electric potential \( V \) at a point in an electric field is the work done in bringing a unit positive charge from infinity to that point, without any acceleration. It is given by:

\[
V = k \cdot \frac{Q}{r}
\]

For multiple point charges, the total potential is the sum of the potentials due to each charge.

# Function Explanations

## 3.1 Setting Up the Environment
- *Function*: setup_environment()
- *Description*: Initializes the plot area and settings for the visualization.
- *Usage*: setup_environment()

## 3.2 Plotting Electric Fields
- *Function*: plot_electric_field(charges, grid_size)
- *Parameters*: 
  - charges: A list of tuples representing charge positions and magnitudes, e.g., [(1, (0, 0)), (-1, (1, 1))].
  - grid_size: Tuple indicating the size of the grid for the field, e.g., (10, 10).
- *Description*: Calculates and visualizes the electric field generated by the specified charges on the grid.
- *Usage*: plot_electric_field([(1, (0, 0)), (-1, (1, 1))], (10, 10))

## 3.3 Plotting Electric Potential
- *Function*: plot_potential(charges, grid_size)
- *Parameters*: Same as plot_electric_field.
- *Description*: Calculates and visualizes the electric potential generated by the specified charges on the grid.
- *Usage*: plot_potential([(1, (0, 0)), (-1, (1, 1))], (10, 10))

# Usage Examples

### Example 1: Visualizing the Electric Field
```python
from visualization_tool import setup_environment, plot_electric_field

setup_environment()
plot_electric_field([(1, (0, 0)), (-1, (1, 1))], (10, 10))
This example sets up the environment and visualizes the electric field due to a positive charge at the origin and a negative charge at (1,1).

Example 2: Visualizing Electric Potential
python
Copy code
from visualization_tool import setup_environment, plot_potential

setup_environment()
plot_potential([(1, (0, 0)), (-1, (1, 1))], (10, 10))



