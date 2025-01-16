# Voice Assistant Web Interface

A modern, interactive web interface for triggering voice assistant functionality, featuring a dynamic network animation background and responsive design.

## Features

- **Interactive Microphone Button**
  - Large, centered microphone button with visual feedback
  - Smooth hover and click animations
  - Pulsing effect animation
  - Status indicator text

- **Dynamic Network Background**
  - Animated particles creating a web-like effect
  - Responsive to screen size
  - Smooth particle movement and connections
  - Gradient background blend

- **Modern UI Elements**
  - Toast notifications for feedback
  - Responsive design for all screen sizes
  - Clean typography and layout
  - Smooth animations and transitions

## Technical Requirements

- Modern web browser with HTML5 Canvas support
- JavaScript enabled
- Backend server capable of handling POST requests to `/trigger` endpoint

## Installation

1. Clone the repository to your local machine
2. Place the files in your web server directory
3. Ensure your backend server is configured to handle POST requests to `/trigger`

## File Structure

```
voice-assistant/
├── index.html    # Main HTML file containing all code
├── README.md     # This documentation file
```

## Usage

1. Open `index.html` in a web browser
2. Click the microphone button to trigger the voice assistant
3. The interface will send a POST request to `/trigger`
4. Status updates will be shown via toast notifications

## Backend Integration

The interface expects a JSON response from the `/trigger` endpoint with the following structure:

```json
{
    "status": "success",
    "message": "Optional message"
}
```

## Customization

### Network Animation

You can customize the network animation by modifying these variables in the JavaScript code:

```javascript
const particleCount = 100;        // Number of particles
const connectionDistance = 150;    // Maximum distance for particle connections
const particleRadius = 2;         // Size of particles
```

### Styling

The interface uses CSS variables for easy customization of colors and animations. Key style elements can be modified in the CSS section:

```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);  // Background gradient
animation: pulse 2s infinite;  // Pulse animation timing
```

## Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Performance Considerations

- The network animation uses HTML5 Canvas for optimal performance
- Particle count can be adjusted based on device capabilities
- Animation frame rate is synchronized with screen refresh rate

## Known Issues

- High particle counts may impact performance on low-end devices
- Toast notifications may stack if triggered in quick succession

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Particle network animation inspired by various canvas demos
- UI design following modern web design principles
- Built with vanilla JavaScript for maximum compatibility

## Support

For support, please open an issue in the repository or contact the development team.
