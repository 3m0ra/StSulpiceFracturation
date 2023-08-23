# StSulpiceFracturation
This repository contains the numerical annexes to Emanuele J. Morotti's Bachelor's degree work, entitled "Caractérisation d'affleurements fracturés par photogrammétrie" and carried out at the University of Neuchâtel's Centre for Hydrogeology (CHYN) under the direction of prof. Benoît Valley.

---
Below is a description of the files.

---
**Planes.csv**

This file contains all the data of all the plans extracted from the cliff treated in the example application of the workflow. The columns of the file include:

- Index: the name of the plan, as generated by the Facets plugin.
- CenterX: the x position of the plane's center (in CH1903+/LV95).
- CenterY: the y position of the plane's center (in CH1903+/LV95).
- CenterZ: the z position of the plane's center (in CH1903+/LV95).
- NormalX: the Cartesian x component of the unit vector normal to the plane.
- NormalY: the Cartesian y component of the unit vector normal to the plane.
- NormalZ: the Cartesian z component of the unit vector normal to the plane.
- RMS: [m] the point-to-plane distance expressed as the root mean squared (RMS).
- Horiz_ext: [m] the horizontal extension of the plane's inscribed rectangle.
- Vert_ext: [m] the vertical extension of the plane's inscribed rectangle.
- Surf_ext: [m^2] the area of the plane's inscribed rectangle.
- Surface: [m^2] the area of the plane.
- Dip dir.: [°] the dip direction of the plane.
- Dip: [°] the dip angle of the plane with respect to the horizontal.

---
**Filtered_planes.csv**

This file contains information regarding the planes used in the analytical part of the thesis. These are the planes included in Planes.csv with a "Surface" field of at least 0.2 m^2. The columns of the file are the same as those in Planes.csv, with the addition of a column:

- Set: the number of the set to which the plane belongs.

---
**St_Sulpice.ipynb**

This document is a Python Jupyter Notebook file. It contains all the code that was used to analyze the data concerning the plans extracted by CloudCompare and Facets (e.g. calculation of spacing between families, creation of figures, etc.). A description is provided in comments directly within the file.
