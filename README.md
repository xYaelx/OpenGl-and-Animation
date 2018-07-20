# OpenGl-and-Animation
This project implement an OpenGL 3D animation game that will consist of a locomotive moving on a track. So it is composed with two components:
1. Drawing a locomotive in OpenGl and directing the camera (point of view) to the point where your mouse points

2. Drawing a rails - The track can be modeled by a parametric closed curve using cubic splines.

The splines are calculated as follow:
- each spline is defined as Spline (class)
- the splines are calculated in SplinesSolver
- all the splines are hosted in TrackSplines

In the Track class we draw the rail by the calculated splines and update the locomotive velocity :)

Usage
- The user can rotate the view around the model by dragging the mouse over the canvas.
- Mouse wheel is used to zoom in and out.
- The user can change the window’s size and alter its ratio, without distorting the
image.
- Pressing ‘p’ toggles wireframe and filled polygon modes.
- Pressing ‘m’ displays the next model.
- Pressing ‘a’ turns the xyz axis on/off.
- The application receives no command line parameters.
 Pressing ‘c’ toggles the camera position.
- Pressing ‘l’ (Bonus) - turns on/off marking the light sources (little spheres will be
displayed at the location of the light sources, which will have only an emittance
attribute – i.e. not affected by the light source itself).
- Pressing the up and down arrows changes the locomotive's speed (note that the
speed can be negative – in which case the locomotive will move backwards).
- Typing a number (greater than zero) and then pressing Enter changes the track.
- Pressing esc closes the application.
