# Shashank_Chavan-Portfolio
Personal Portfolio Website | Showcasing my web development skills, projects, and career highlights. Built with modern design principles and responsive layouts for an impressive job-hunting presence.

=================
Animation Details
=================
Particle Animation for Full-Screen Background
This project adds an interactive particle animation effect to your website's background. It uses Particles.js, a lightweight JavaScript library, to create dynamic particles that move around the screen and react to user interactions.

Features:
Full-Screen Animation: The particle effect fills the entire viewport (width and height).

Interactive: Particles move away from the cursor when hovered, providing an engaging effect.

Customizable: Easy to modify particle size, color, and speed.

How to Implement:
Step 1: Include the Particles.js Library
Add the following script tag in the <head> section of your HTML file to load the Particles.js library:

html
Copy
Edit
<script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js"></script>
Step 2: Create the Particle Container
Inside the <body> of your HTML file, add the following <div> to serve as the container for the particle animation:

html
Copy
Edit
<div id="particles-js"></div>
Step 3: Style the Container
To make the particles fill the entire screen, add the following CSS in your stylesheet or <style> tag:

css
Copy
Edit
#particles-js {
  position: fixed;  /* Fix the position to stay in place while scrolling */
  top: 0;
  left: 0;
  width: 100vw;  /* Full viewport width */
  height: 100vh; /* Full viewport height */
  background-color: #000;  /* Optional: background color for contrast */
  z-index: -1;  /* Ensure particles stay behind other content */
}
Step 4: Add the Particle Configuration
Just before the closing </body> tag, add the following script to configure the particle behavior. You can customize the number of particles, size, and interactivity as needed:

html
Copy
Edit
<script>
  particlesJS("particles-js", {
    particles: {
      number: {
        value: 100,  // Number of particles
        density: {
          enable: true,
          value_area: 800
        }
      },
      shape: {
        type: "line",  // Particle shape as line
        stroke: {
          width: 2,
          color: "#ffffff"  // White color for the lines
        }
      },
      size: {
        value: 3,  // Size of the particles (small lines)
        random: true
      },
      move: {
        enable: true,
        speed: 1,  // Speed of particle movement
        direction: "none",
        random: true,
        straight: false,
        out_mode: "out"
      }
    },
    interactivity: {
      detect_on: "window",
      events: {
        onhover: {
          enable: true,
          mode: "repulse"  // Particles repulse on hover
        }
      }
    },
    retina_detect: true
  });
</script>
Step 5: Customize the Particle Effect
Feel free to adjust the configuration parameters:

value in number: Controls the number of particles on the screen.

size in size: Controls the size of the particles.

stroke in shape: Controls the thickness and color of the lines.

speed in move: Controls how fast the particles move.

Example HTML File:
html
Copy
Edit
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Portfolio</title>
  <!-- Load Particles.js -->
  <script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js"></script>
  <style>
    #particles-js {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background-color: #000;
      z-index: -1;
    }
  </style>
</head>
<body>

  <!-- Particle container -->
  <div id="particles-js"></div>

  <!-- Your website content goes here -->

  <!-- Particle configuration script -->
  <script>
    particlesJS("particles-js", {
      particles: {
        number: {
          value: 100,
          density: {
            enable: true,
            value_area: 800
          }
        },
        shape: {
          type: "line",
          stroke: {
            width: 2,
            color: "#ffffff"
          }
        },
        size: {
          value: 3,
          random: true
        },
        move: {
          enable: true,
          speed: 1,
          direction: "none",
          random: true,
          straight: false,
          out_mode: "out"
        }
      },
      interactivity: {
        detect_on: "window",
        events: {
          onhover: {
            enable: true,
            mode: "repulse"
          }
        }
      },
      retina_detect: true
    });
  </script>

</body>
</html>
Conclusion:
This setup creates a full-screen particle background with dynamic lines that interact with the mouse cursor. It's easy to integrate into any portfolio or personal website. Feel free to customize the particle behavior to fit your design and project needs.

For more customization options, check the Particles.js documentation.
=====================================================================

