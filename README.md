Interactive 3D Orrery: Nearby Planets
This is an interactive 3D Orrery built using HTML, CSS, and JavaScript with the Three.js library. It simulates the solar system with a focus on nearby planets of Earth—Mercury, Venus, Earth, and Mars. The project allows users to explore the planets, view detailed information on them, and experience a visually engaging space environment.

Features
3D Representation of the Solar System: Visualizes the Sun, nearby planets (Mercury, Venus, Earth, Mars), their orbits, and moons.
Interactive Planet Info Box: Click on a planet to see details such as size, distance from the Sun, and any associated moons.
Planet Labels: Toggle labels for planets to identify them easily.
Responsive Camera Controls: Use mouse controls to pan, zoom, and rotate around the solar system.
Realistic Background Stars: A star field adds depth to the scene for an immersive space experience.
Mobile-Compatible: Responsive controls and UI, making it accessible on various devices.
Installation
1. Clone the Repository
bash
Copy code
git clone [https://github.com/your-username/3d-orrery.git](https://github.com/iblameatharv/OrreySpaceApp)
2. Open the Project
Navigate to the project directory and open index.html in your browser.

bash
Copy code
cd 3d-orrery
open index.html
Alternatively, you can drag and drop index.html into any modern web browser.

Usage
Controls:
Start Simulation: Starts the solar system simulation, allowing planets to orbit around the Sun.
Stop Simulation: Stops the simulation, freezing the planets in their orbits.
Reset View: Resets the camera to the original position for an overview of the system.
Toggle Labels: Show or hide labels for each planet.
Planet Information:
Click on a planet to display detailed information in the info box. You can see:

Planet Name
Planet Size
Distance from the Sun
Moons (if any)
Moons:
Earth’s Moon is displayed with size and orbit.
Mars’ moons Phobos and Deimos are also rendered with correct positioning and orbiting motion.
Dependencies
Three.js: The JavaScript 3D library used for rendering the solar system and handling 3D object manipulations.
Project Structure
bash
Copy code
3d-orrery/
│
├── index.html            # Main entry point for the web app
├── README.md             # Project documentation
└── assets/               # (Optional) Assets like images, textures, if any
Customization
Adding More Planets:
You can add additional planets by calling the createPlanet() function in index.html. For example:

javascript
Copy code
createPlanet('Jupiter', 50, 350, 0.4, [{ name: 'Europa', size: 7, distance: 40 }, { name: 'Ganymede', size: 10, distance: 50 }]);
Modifying Planet Properties:
You can modify the size, speed, and distance of planets by changing the parameters in the createPlanet() function:

Size: Controls the size of the planet.
Distance: How far the planet is from the Sun.
Speed Factor: Controls the orbiting speed.
Changing Star Density:
To change the density of stars in the background, modify the value in the addStars() function.

javascript
Copy code
for (let i = 0; i < 10000; i++) {
  const x = THREE.MathUtils.randFloatSpread(2000);
  const y = THREE.MathUtils.randFloatSpread(2000);
  const z = THREE.MathUtils.randFloatSpread(2000);
  starVertices.push(x, y, z);
}
Future Enhancements
Full Solar System Representation: Expand to include all planets and dwarf planets.
Dynamic Planetary Data: Fetch live planetary data from APIs like NASA’s.
Advanced Camera Features: Implement smooth transitions when focusing on specific planets.
Contributing
Feel free to fork this repository, make improvements, and create pull requests. Contributions are welcome!

License
This project is open source and available under the MIT License.

