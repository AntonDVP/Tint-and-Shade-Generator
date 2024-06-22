# Tint-and-Shade-Generator

A web-based tool for generating and visualizing color systems based on a chosen base color. This project allows users to create a harmonious set of tints and shades, providing a comprehensive color palette for design projects.

![Tint and Shade Generator](https://raw.githubusercontent.com/AntonDDVP/tint-and-shade-generator/assets/Tint-And-Shade-Generator.jpg)

## Features

- 🎨 Interactive color picker and HEX code input
- 🔢 Adjustable number of tints and shades (2-20)
- ⚡ Real-time color system generation
- ♿ WCAG 2.2 contrast ratio calculations for accessibility
- 💾 Export options: Image (PNG), Text (TXT), Table (CSV), and Design Tokens (JSON)
- 📱 Responsive design for both desktop and mobile use

## How It Works

### Color Generation Algorithm

The tool uses the tinycolor.js library to handle color manipulations. The generation process works as follows:

1. The user selects a base color using the color picker or by entering a HEX code.
2. The user chooses the number of steps (2-20) for tints and shades.
3. The system generates tints by mixing the base color with white in incremental steps.
4. The system generates shades by mixing the base color with black in incremental steps.
5. The main color (base color) is placed in the center of the generated palette.

### Color Naming

The tool attempts to name the base color by comparing it to a predefined list of common color names. It uses a simple distance calculation in the RGB color space to find the closest named color.

### Accessibility Information

For each generated color, the tool calculates and displays WCAG 2.2 contrast ratios against both white and black backgrounds. This helps designers ensure their color choices meet accessibility standards.

## Technologies Used

- HTML5
- CSS3 (with Tailwind CSS for styling)
- JavaScript (ES6+)
- External libraries:
  - [tinycolor.js](https://github.com/bgrins/TinyColor) for color manipulation
  - [html2canvas](https://html2canvas.hertzen.com/) for image export functionality

## Export Options

1. **Image (PNG)**: Captures the entire color palette as a PNG image.
2. **Text (TXT)**: Exports color information including labels, HEX codes, and accessibility data in a plain text format.
3. **Table (CSV)**: Provides a comma-separated values file with color information, suitable for spreadsheet applications.
4. **Design Tokens (JSON)**: Exports the color palette as a JSON file, following a design token structure for easy integration with design systems.

## Getting Started

To use this tool, simply open the HTML file in a modern web browser. No server-side setup is required as all processing is done client-side.

```bash
git clone https://github.com/yourusername/tint-and-shade-generator.git
cd tint-and-shade-generator
open index.html
```

## Future Enhancements

- [ ] Add support for different color models (RGB, HSL, etc.)
- [ ] Implement color palette suggestions based on color theory
- [ ] Provide more advanced export options (e.g., Sass variables, CSS custom properties)
- [ ] Enhance the color naming algorithm for more accurate results
- [ ] Create a Figma plugin version of this tool for seamless integration with the Figma design workflow

Contributions and suggestions for improvements are welcome! Feel free to open an issue or submit a pull request.

## Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request

## License

Distributed under the Apache-2.0 license. See `LICENSE` for more information.

## Acknowledgements

This tool was created with the assistance of Claude 3.5 Sonnet, an AI language model by Anthropic. Claude provided guidance and generated 99% of the code and documentation for this project, demonstrating the potential of AI-assisted development in creating functional and well-documented tools.

---

Made with ❤️ and AI 🤖