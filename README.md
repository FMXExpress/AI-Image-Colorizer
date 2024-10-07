# AI Image Colorizer + Replicate API

This is a desktop application built with DelphiFMX that allows you to upload a grayscale image and automatically colorize it using the [Replicate API](https://replicate.com/). The app provides an easy-to-use interface for selecting images, displaying the original grayscale image alongside the colorized version, and managing the processing status.

## Features

- **Image Upload**: Select a grayscale image (`.png`, `.jpg`, or `.jpeg`).
- **Image Display**: View the original and colorized images side by side.
- **Status Updates**: See real-time status messages while the image is being processed.
- **Replicate API**: Uses the `piddnad/ddcolor` model from Replicate for colorization.
- **Responsive Design**: Clean, responsive layout built with DelphiFMX.
- **Error Handling**: Displays error messages if image processing fails.

## Prerequisites

1. **Python**: This application requires Python to be installed on your system.
2. **Replicate API Key**: You will need a [Replicate API Key](https://replicate.com/account) to run the app. Once you have the key, set it as an environment variable:
   ```bash
   export REPLICATE_API_TOKEN="your_replicate_api_key"
   ```

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/ai-image-colorizer-fmx.git
   cd ai-image-colorizer-fmx
   ```

2. **Install required Python packages**:
   Ensure that you have `replicate` installed:
   ```bash
   pip install replicate
   ```

3. **Run the Application**:
   You can run the application directly using Python:
   ```bash
   python colorizier.py
   ```

## Usage

1. **Upload an Image**: Click the "Select" button and choose a grayscale image (`.png`, `.jpg`, or `.jpeg`) from your local system.
2. **Wait for Processing**: The status bar will show updates on the colorization progress. The colorization is done using the `piddnad/ddcolor` model from Replicate.
3. **View the Results**: Once the colorization is complete, the original grayscale image and the newly colorized image will be displayed side by side.

## Project Structure

```bash
ai-image-colorizer-fmx/
│
├── colorizer.py            # Main entry point for the application
├── Air.style          # DelphiFMX style used for the UI
└── README.md          # This README file
```

## Models Used

The application uses the [piddnad/ddcolor](https://replicate.com/piddnad/ddcolor) model for colorizing grayscale images. You can view more details about the model on its [Replicate page](https://replicate.com/piddnad/ddcolor).

## Notes

- **API Limitations**: Ensure that your Replicate account has enough credits to run the colorization model.
- **Performance**: The image processing time will vary depending on the size of the image and the speed of the Replicate model.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
