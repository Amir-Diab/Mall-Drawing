# Mall Drawing
## About
Drawing a multi-storey mall, inside and outside environment with moving ability using OpenGL in C++.

Me and my teammate Muhammad Hreden have done this work based on legacy OpenGL, starting from the basic drawing functions presented by [NeHe's website](http://nehe.gamedev.net/). The project was built and tested using Visual Studio 2019.

We included textures, models, lighting and a simple logic for moving to seem rather realistic. Before drawing anything, we created a general class `Draw` that has a set of functions which are responsible for drawing all important primitive shapes that any complix object may made from. These functions accept position, lengths, lighting normal direction, texture and texture mapping as parameters. This is very helpful during drawing the environment as a kind of abstraction. Repeatedly drawn objects were also arranged in functions so that they become easier to be drawn.

## What was drawn? 
The mall consists of two floors and two other underground floors, with a small garden and a street arround.
The first and second floors contain clothes markets, whereas, the first basement contain resturants and the second one is a car parking.
You can move between the floors in three ways :
- Normal stairs: your height is automatically fixed while moving on them.
- Electric stairs: for carrying up and down.
- Elevators: by standing inside and press buttons.

## Screenshots
![mall at day](https://user-images.githubusercontent.com/57280180/159220596-693820b5-ecfe-424b-9ecb-53e452845b2d.jpg)
![mall at night](https://user-images.githubusercontent.com/57280180/159220640-59f4cf18-aad6-4b7f-a2d3-5688cc7c6943.jpg)
![inside](https://user-images.githubusercontent.com/57280180/159220680-1fec37d0-6b8a-497e-a254-6f4ca5f64207.jpg)
![first basement](https://user-images.githubusercontent.com/57280180/159220710-068ab486-1945-44a8-bb2b-6fe8839afdf5.jpg)
![second basement](https://user-images.githubusercontent.com/57280180/159220531-9187ce85-653b-40a0-9ca5-6b91fe6045f3.jpg)
![third person](https://user-images.githubusercontent.com/57280180/159220563-600e1219-7f7e-40b6-a5ba-82ab3a5ba22e.jpg)

## Control
For moving:
- **W:** forward
- **S:** backward
- **A:** left
- **D:** right
- **Upwards Arrow ↑:** up
- **Downwards Arrow ↓:** down

- **Mouse** is used for yaw rotating.

- **E:** move elevators up
- **Q:** move elevators down
- **T:** switch between first person (FP) and third person (TP) perspectives
- **N:** switch between day and night modes
