# Mapbox GL JS Overlay Example

This repository contains an example of how to use Mapbox GL JS to overlay an image on a map, with functionality to drag and resize the image. The project demonstrates the integration of image overlays in a Mapbox map and includes interactive features for a rich user experience.

## Description

This example showcases the following:
- Integration of Mapbox GL JS for interactive maps.
- Adding an image overlay to a map.
- Allowing users to drag and resize the image overlay.
- Using markers to indicate corners of the image for resizing.

The provided code is a great starting point for developers looking to incorporate image overlays into their Mapbox GL JS projects with interactive features.

## Features

- **Interactive Map**: Utilizes Mapbox GL JS to create an interactive map.
- **Image Overlay**: Adds an image overlay to the map.
- **Draggable Image**: Allows users to drag the image overlay across the map.
- **Resizable Image**: Users can resize the image overlay using draggable corner markers.
- **Custom Styling**: Easily customizable markers and image opacity.

## Setup Instructions

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/mapbox-gl-js-overlay-example.git
    cd mapbox-gl-js-overlay-example
    ```

2. **Open the `index.html` file**:
    - Use your preferred method to serve the `index.html` file locally. For example, you can use VS Code's Live Server extension or a simple HTTP server with Python:
      ```bash
      python -m http.server
      ```

3. **Replace the Mapbox Access Token**:
    - Open `index.html` in your text editor.
    - Replace the `mapboxgl.accessToken` with your own Mapbox access token.
    - Obtain a token from [Mapbox](https://account.mapbox.com/access-tokens/).

4. **Open the Map**:
    - Navigate to `http://localhost:8000` (or the appropriate URL provided by your HTTP server) to view and interact with the map.

## Code Explanation

### HTML Structure

The HTML file includes the necessary Mapbox GL JS CSS and JS files, sets up the map container, and initializes the Mapbox map.

### JavaScript Logic

- **Map Initialization**:
    ```javascript
    const map = new mapboxgl.Map({
      container: 'map',
      style: 'mapbox://styles/mapbox/streets-v11',
      center: [74.2778593, 31.4809879], // Initial center coordinates
      zoom: 15
    });
    ```

- **Image Overlay**:
    - Adds an image overlay to the map using the `map.addSource` and `map.addLayer` methods.

- **Markers for Resizing**:
    - Creates draggable markers at the corners of the image for resizing.

- **Dragging and Resizing Logic**:
    - Implements `mousedown`, `mousemove`, and `mouseup` event listeners to handle dragging and resizing of the image overlay.

### Customization

- **Markers**:
    - Customize the markers by editing the CSS in the `<style>` section.
- **Image Opacity**:
    - Adjust the image opacity by changing the `raster-opacity` property in the `map.addLayer` method.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any enhancements or bug fixes.

## Keywords

Mapbox, Mapbox GL JS, Image Overlay, Interactive Map, Draggable Image, Resizable Image, JavaScript, HTML, Web Development

