# Twitch Sub Goal Widget for StreamElements

A sleek and customizable **Twitch Subscriber Goal Widget** designed for StreamElements overlays. This widget dynamically updates subscriber progress, features animations for low progress, and celebrates when the goal is reached.

## Features
- **Progress Bar**: Displays the current progress toward the subscriber goal.
- **Low Progress Animation**: Pulsing effect when progress is below 5%.
- **Celebration Effect**: Confetti animation when the goal is achieved.
- **Customizable Colors**: Easily adjust colors via CSS variables.
- **Real-Time Updates**: Automatically updates with new subscriber events.

## How It Works
1. The widget listens for `subscriber-latest` events from StreamElements.
2. Updates the progress bar dynamically as new subscribers are added.
3. Triggers a confetti celebration when the goal is reached.

## Installation
1. Copy the code from `html.html` into a new widget in your StreamElements overlay.
2. Adjust the `config` object in the `<script>` section to set your subscriber goal:
   ```javascript
   let config = {
     goal: 50, // Set your subscriber goal
     current: 0, // Current subscriber count
     minVisibleWidth: 2 // Minimum visible width for the progress bar
   };
   ```
3. Save and add the widget to your overlay.

## Customization
You can customize the widget's appearance by modifying the CSS variables in the `<style>` section:
```css
:root {
  --primary-color: #9147ff; /* Main color */
  --secondary-color: rgba(20, 20, 25, 0.8); /* Background color */
  --text-color: #ffffff; /* Text color */
  --progress-color: #5a3da8; /* Progress bar gradient */
  --highlight-color: #bf94ff; /* Highlight color */
  --empty-color: rgba(255, 255, 255, 0.1); /* Empty progress bar color */
}
```

## Demo

## Technologies Used
- **HTML/CSS**: For structure and styling.
- **JavaScript**: For dynamic updates and animations.

## License
This project is licensed under the MIT License. Feel free to use, modify, and share it.