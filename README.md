<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cognitive &amp; Perceptual Studies — Intake Survey README</title>
<style>
  body {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    line-height: 1.6;
    color: #333;
    max-width: 800px;
    margin: 0 auto;
    padding: 2rem;
  }
  h1, h2 {
    color: #111;
    border-bottom: 1px solid #eaeaea;
    padding-bottom: 0.3em;
    margin-top: 1.5em;
  }
  h1 {
    margin-top: 0;
  }
  code {
    background-color: #f6f8fa;
    padding: 0.2em 0.4em;
    border-radius: 3px;
    font-family: ui-monospace, SFMono-Regular, "SF Mono", Menlo, Consolas, "Liberation Mono", monospace;
    font-size: 85%;
  }
  ul, ol {
    padding-left: 2em;
  }
  li {
    margin-bottom: 0.5em;
  }
</style>
</head>
<body>

  <h1>Cognitive &amp; Perceptual Studies — Intake Survey</h1>

  <p>An interactive, browser-based psychological horror fiction piece masquerading as a clinical intake survey. As the user progresses through the seemingly innocuous multiple-choice questions, the interface gradually deteriorates, introducing escalating visual glitches, eerie procedural audio, and an underlying sense of dread.</p>

  <h2>👁️ Overview</h2>

  <p>This project is a self-contained, single-file web application built with HTML, CSS, and Vanilla JavaScript. It requires no external image or audio assets, relying entirely on CSS effects, inline SVGs, and the Web Audio API to create its atmosphere.</p>

  <p><strong>Content Warning:</strong> This experience contains themes of memory loss, identity dissociation, psychological unease, and features mild flashing/glitching visual effects.</p>

  <h2>✨ Features</h2>

  <ul>
    <li><strong>Dynamic "Dread" System:</strong> The environment reacts to the player's progression. As the survey advances, the CSS filters, color palettes, and glitch frequency intensify.</li>
    <li><strong>Procedural Horror Audio:</strong> A fully synthesized soundtrack built with the Web Audio API featuring:
      <ul>
        <li>Dissonant, low-frequency beating drones.</li>
        <li>A procedural "breathing" white noise filter that accelerates with the dread level.</li>
        <li>Startling audio stings synced with visual chromatic aberration glitches.</li>
      </ul>
    </li>
    <li><strong>Interactive SVG Background:</strong> A subtle eye graphic that follows the user's cursor, growing more visible as the dread level increases.</li>
    <li><strong>Robust Customization Menu:</strong> Users can tailor their experience via the settings toggle:
      <ul>
        <li><strong>Themes:</strong> Clinical (Default), Crimson, and The Void.</li>
        <li><strong>Typography:</strong> Toggle between formal Serif and terminal Monospace fonts.</li>
        <li><strong>CRT Scanlines:</strong> Adjust the intensity of the retro CRT overlay.</li>
      </ul>
    </li>
    <li><strong>Accessibility:</strong> Full support for <code>prefers-reduced-motion</code>. Users can also manually toggle a "Reduced Motion" mode in the settings or on the consent screen to disable flashing glitches and eye tracking while preserving the narrative experience.</li>
  </ul>

  <h2>🚀 How to Run</h2>

  <ol>
    <li>Download or copy the <code>index.html</code> file.</li>
    <li>Open <code>index.html</code> in any modern web browser (Chrome, Firefox, Safari, Edge).</li>
    <li><strong>Note:</strong> For the full experience, ensure your system audio is turned on and you click the "sound: off" toggle in the bottom right corner to initialize the Web Audio engine.</li>
  </ol>

  <h2>🛠️ Technical Details</h2>

  <ul>
    <li><strong>No Dependencies:</strong> Zero external libraries, frameworks, or asset files.</li>
    <li><strong>State Management:</strong> A simple internal state object tracks the user's answers, current question index, dread level, and configuration preferences.</li>
    <li><strong>Web Audio API:</strong> All sound effects and ambient noise are generated in real-time using <code>OscillatorNode</code>, <code>GainNode</code>, and <code>BiquadFilterNode</code>.</li>
    <li><strong>CSS Variables:</strong> Extensive use of CSS variables (<code>--dread</code>, <code>--accent-live</code>, <code>--bg</code>) allows for seamless, smooth transitions between themes and atmosphere states.</li>
  </ul>

  <h2>📜 Disclaimer</h2>

  <p>This is a fictional interactive horror story. No data is collected, transmitted, or stored anywhere. What happens in the survey, stays in the survey.</p>

</body>
</html>
