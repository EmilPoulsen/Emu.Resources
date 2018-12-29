# Elastic Gridshell Formation

## Description
This example demonstrates how Emu can be used to simulate the formation process of an elastic gridshell and visualize bi-axial moments and torsion caused by internal stresses as diagrams. The structure starts out flat on the ground and is subsequently transformed to its erected state by pulling the support points towards the middle. By using the `Lath Elements`, moments are not being transferred between the two directions of the grid, simulating a scissor like behavior in the nodes.

## Instructions
1. Download the [definition](Emu_ElasticGridshellFormation.gh)
2. Open the definition in Rhino 5/6
3. Hit the rebuild button connected to the model component.
4. Set the "Support location" slider to 1.
5. The DiagramViewer is blocked by a Data Dam component to make the simulation run faster.
6. Double click on the Timer component to start the simulation.
7. Move the "Support location" slider to 0.5 (carefully and not too fast!). This will move the supports towards the centroid.
8. When the simulation has converged (when nothing is moving and the residual forces/moments approach zero), double click again on the Timer component to stop the simulation.
9. Now enable the DiagramViewer component by hitting play on the data dam to visualize bi-axial bending and torsion.

Extra:
10. Change the Element Type in the Diagram Viewer to view moments about different axes (minor/major/torsion).
11. Use the Element Index selector to visualize diagrams of two different groups representing the two directions of the grid.
12. To restart the simulation, mote the supports back to its original state (see step 4) and hit the Reset button on the Dynamic Relaxation component.

## Preview
TODO

![Preview of output](Emu_ElasticGridshellFormation_Preview.jpg)

![Preview of Grasshopper definition](Emu_ElasticGridshellFormation_Definition.jpg)
