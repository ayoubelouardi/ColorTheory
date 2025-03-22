# Video Color Palette Generator

This HTML, CSS, and JavaScript code implements a web application that generates color palettes from a video frame. Users upload an image, and the application analyzes it to provide various color harmonies, including:

* **Average Color:** The overall average color of the image.
* **Dominant Colors:** The top three most frequent colors.  Users can select a dominant color to base other harmonies on.
* **Monochromatic:** Shades and tints of a single hue.
* **Analogous:** Three colors adjacent on the color wheel.
* **Complementary:** Colors opposite each other on the color wheel (for both average and dominant colors).
* **Split-Complementary:** Colors from either side of a complementary color pair.
* **Triadic:** Three colors equally spaced on the color wheel.
* **Tetradic:** Two sets of complementary color pairs.
* **Square:** Four colors evenly spaced on the color wheel.

## Features

* **Image Upload:** Users can select an image file (supports common image formats).
* **Color Enhancement:**  Provides controls for adjusting brightness, saturation, and contrast, with an option for automatic enhancement.
* **Color Display:**  Displays color swatches with HEX codes and copy-to-clipboard functionality.
* **Dark Mode Support:**  Automatically detects and adapts to the user's system preference for dark mode.
* **Responsive Design:**  The layout adapts to different screen sizes, including mobile devices.
* **Color Harmony Algorithms:**  Implements algorithms to calculate various color harmonies based on color theory.
* **Color Selection:** Allows users to select from the dominant colors to generate harmonies around the selected color.

## Technologies Used

* **HTML:**  Provides the structure and content of the web page.
* **CSS (Tailwind CSS):**  Used for styling the page with a utility-first approach.
* **JavaScript:**  Handles user interactions, image processing, color analysis, and UI updates.

## How it Works

1.  **Image Upload:** The user selects an image using the file input.
2.  **Image Analysis:** The JavaScript code analyzes the image using a canvas element to extract color information.  It calculates the average color and identifies the top three dominant colors.  The image is resized to a maximum of 300 pixels on either dimension to improve performance.
3.  **Color Harmony Calculation:**  The code calculates the various color harmonies (monochromatic, analogous, complementary, etc.) using algorithms based on color theory.  It converts RGB to HSL for calculations and back to RGB for display.
4.  **UI Update:** The results are displayed on the page with color swatches, HEX codes, and copy buttons.
5.  **Copy to Clipboard:**  Users can copy the HEX codes to their clipboard.
6.  **Color Enhancement:**  The color enhancement features use HSL color space for better manipulation of brightness, saturation and contrast.  Auto-enhancement boosts lightness for dark colors and saturation for dull colors.

## Code Structure

The code is well-structured and commented to improve readability.  The main functions include:

*   `handleImageUpload()`: Handles image upload and initiates the analysis process.
*   `analyzeImage()`: Analyzes the image data to extract color information.
*   `calculateAverageColor()`: Calculates the average RGB color of the image.
*   `findDominantColor()`: Finds the top three most frequent colors.
*   `calculateComplementaryColor()`: Calculates the complementary color.
*   `rgbToHex()`: Converts RGB to HEX color codes.
*   `createColorSwatch()`: Creates a color swatch element for display.
*   `updateColorUI()`: Updates the UI with the calculated color information.
*   `copyToClipboard()`: Copies text to the clipboard.
*   `rgbToHsl()`, `hslToRgb()`:  RGB to HSL and HSL to RGB color space conversions.
*   Other functions for calculating various color harmonies.

The code also includes dark mode detection and responsive design using Tailwind CSS.


This README provides a comprehensive overview of the code's functionality, features, and implementation details.  The code itself is well-commented and easy to understand.
