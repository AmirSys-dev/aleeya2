## Brand & Style

This design system is built on the narrative of digital decay and psychological obsession. It draws heavily from **Brutalism** and **Cyber-Horror** aesthetics, creating an environment that feels unstable, intrusive, and visceral. The interface should feel like a corrupted terminal—a window into a mind that is simultaneously meticulous and unraveling.

The visual language utilizes high-contrast transitions, "glitch" artifacts, and a heavy emphasis on claustrophobic negative space. Every interaction must evoke a sense of unease, as if the UI is watching the user back. Key stylistic hallmarks include:
- **Digital Distortion:** Non-destructive glitch effects on hover and page transitions.
- **Vignette & Grain:** A persistent CRT-style scanline overlay and deep inner-shadow vignettes to draw focus toward the "altar" of the content.
- **Obsessive Repetition:** Micro-copy or background patterns that repeat phrases or "static" to reinforce the yandere theme.

## Layout & Spacing

The layout follows a **Fixed Grid** model to create a sense of rigid, obsessive control. Use a 12-column grid for desktop with 24px gutters.

- **Asymmetry:** Occasionally break the grid with "corrupted" elements that bleed off-canvas or overlap other containers to suggest a loss of digital integrity.
- **Tight Margins:** Use generous outer margins (40px+) to create a "boxed-in" feeling, isolating the content in the center of the dark screen.
- **Mobile Reflow:** On mobile devices, transition to a single-column layout with 16px margins, maintaining the heavy vignette to prevent the screen from feeling too open.

## Elevation & Depth

Standard shadows are prohibited. In this design system, depth is communicated through **Tonal Layering** and **Negative Light.**

- **Stacking:** Surfaces do not "float"; they are carved out of the void. Higher hierarchy elements use slightly lighter fills (#1A1A1A) rather than shadows.
- **Inner Glow:** Instead of drop shadows, use a 1px inner border or a faint red glow (primary color at 10% opacity) for active containers.
- **CRT Scanlines:** A global fixed-position overlay with a repeating linear gradient creates the texture of an old monitor.
- **Vignette:** A `radial-gradient` overlay on the `body` element (from transparent center to black edges) must be present at all times to keep the focus claustrophobic.

## Components

### Buttons
- **Primary:** Stark #8B0000 background with #F5F5F5 text. Hover state triggers a high-frequency flicker animation and a slight horizontal "shake" glitch.
- **Secondary:** Ghost style with a 1px #393939 border. On hover, the border turns Crimson and the background fills with a 5% red tint.

### Cards
- Simple #0E0E0E boxes with no rounded corners. 
- Hovering over a card should trigger a "static" noise texture overlay and reveal a "Blood Splatter" icon variant in the corner.

### Input Fields
- Underline-only inputs using #393939. When focused, the line turns #8B0000 and pulses slowly like a heartbeat.

### Iconography
- Use thin-stroke, sharp-edged icons. 
- Specialized "Obsession" set: standard icons (like 'Heart' or 'User') should have "distressed" or "splattered" variants that appear on interaction.

### Interactive Presets
- **Flicker:** A CSS keyframe animation that toggles opacity between 0.8 and 1.0 at irregular intervals.
- **Scanline Scroll:** A slow vertical animation of a high-contrast line moving down the screen to mimic a refreshing monitor.