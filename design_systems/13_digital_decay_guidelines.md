## Brand & Style
The brand personality is visceral, unsettling, and intentionally provocative. This design system is built for a personal portfolio that leans into the "Creepypasta" aesthetic—specifically drawing from psychological horror and early internet urban legends. The target audience includes creative collaborators and peers who appreciate dark, experimental, and avant-garde digital art.

The design style is a fusion of **Digital Brutalism** and **Glitch Aesthetics**. It leverages high-contrast environments to evoke a sense of isolation and digital decay. Key visual motifs include:
- **CRT Scanlines:** A persistent overlay that gives the UI a "found footage" or legacy monitor feel.
- **Vignette:** Heavy darkening at the screen edges to focus the user’s gaze and create a claustrophobic atmosphere.
- **Controlled Glitch:** Subtle CSS displacements and chromatic aberration on hover states to suggest a system that is malfunctioning or haunted.

## Layout & Spacing
The layout follows a **Fixed Grid** model to create a sense of order that feels rigid and "trapped."

- **Desktop (1440px+):** A 12-column grid with a wide 4rem margin. This creates a "stage" in the center of the dark screen.
- **Reflow:** Layouts should favor asymmetrical compositions. Content should often be pushed to the edges or centered with excessive whitespace (blackspace) to emphasize isolation.
- **Spacing Rhythm:** Use large vertical gaps (`stack-lg`) between sections to force the user to scroll through the "darkness," building tension before the next piece of content appears.
- **Mobile:** Transition to a 4-column grid with 1rem margins. Elements should stack vertically, maintaining the high-contrast isolation.

## Elevation & Depth
This design system avoids traditional drop shadows and soft blurs to maintain a "flat" yet layered digital environment.

- **Tonal Layers:** Depth is created through opacity rather than shadow. Use semi-transparent Ash Gray overlays (10-20% opacity) for container backgrounds to make them feel like glass or a HUD.
- **Scanline Overlay:** A fixed position `div` with a repeating linear gradient (black and transparent) covers the entire viewport to simulate a CRT monitor.
- **Vignette:** A radial gradient from `transparent` at the center to `black` at the extreme edges (80% opacity) is applied to the main viewport.
- **Redaction:** Use solid Blood Crimson or Black blocks to "redact" or hide information until hover, creating an interactive element of mystery.

## Components
Consistent styling for core elements:

- **Buttons:** Solid Ash Gray borders with Stark White text. On hover, the background fills with Blood Crimson Red and the text triggers a brief "glitch" animation (rapid X-axis translation).
- **Chips/Tags:** Monospaced Space Mono text contained within a simple Crimson Red border. No background fill.
- **Input Fields:** A single bottom border in Ash Gray. When focused, the border turns Crimson Red and a subtle "flicker" animation is applied to the placeholder text.
- **Cards:** Simple rectangular containers with a 1px Ash Gray border. Images inside cards should have a grayscale filter by default, transitioning to full color with a slight red tint on hover.
- **Lists:** Bullet points are replaced with "X" marks or red dashes.
- **Checkboxes:** Square boxes that, when checked, are filled with a Blood Crimson "X" rather than a tick mark.
- **Custom Component (The Glitch Container):** A container that occasionally "jitters" its content using CSS keyframes, used for featured portfolio pieces or high-impact statements.