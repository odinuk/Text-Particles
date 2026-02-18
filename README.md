Interactive Particle Text
A canvas-based particle system that renders text as thousands of individual particles with organic, physics-driven behaviour. Particles flock, explore, and settle into letterforms — and scatter when you move your mouse over them.
What It Does
Text is sampled as pixel data from an offscreen canvas, then each visible pixel becomes a particle with its own personality traits (energy, curiosity, patience). When text changes, particles go through a lifecycle: flocking → exploring → resolving → idle, creating fluid transitions between messages.
Mouse interaction pushes particles away with a repulsion force, and they grow in size and turn green (#AF0) as they react.
Features

Text morphing — particles transition between multiple text messages with staggered, organic animations
Mouse repulsion — particles scatter and resize based on cursor proximity
Particle personalities — each particle has randomised energy, curiosity, and patience values that affect its movement
Control panel — real-time sliders for tweaking every parameter (particle behaviour, flocking, physics, mouse interaction, text settings)
Presets — Default, Gentle Waves, Explosive Entrance, Smooth Transitions, Chaotic Motion
Responsive — adapts to window resize

Usage
Open index.html in a browser. No build step or dependencies — just a single HTML file.
Controls:

Message — cycle through text messages
Regenerate — replay the current text animation
Controls — toggle the parameter panel

Configuration
All parameters are exposed in the control panel and defined in the config object. Key groups:
GroupControlsParticle PersonalityEnergy range, curiosity range, patience variationFlocking BehaviorWave strength, exploration duration/intensity, resolve delayMovement PhysicsVelocity damping, initial force, homing strength, wanderingMouse InteractionRadius, repulsion forceAnimation TimingsLift-off delay, dying duration, opacity fade rateText SettingsFont size, point spacing, line height
Tech
Vanilla HTML/CSS/JS with Canvas 2D. Uses Satoshi via Google Fonts.
Customisation
Edit the texts array in the script to change the messages. Adjust config defaults or create new presets in the presets object.
