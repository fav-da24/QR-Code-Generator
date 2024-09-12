# QR Code Generator

A Python script that generates QR codes from user-provided data and saves them as PNG images. Optionally, the script can display the generated QR code image.

## Features

- Generate QR codes from user-input data.
- Save the generated QR code as a PNG image.
- Optionally display the QR code image after generation.

## Prerequisites

- Python 3.x
- Required Python packages

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/fav-da24/QR-Code-Generator.git
   cd qr-code-generator
   ```

2. **Set up a virtual environment (optional but recommended):**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required packages:**

   This project requires the `qrcode` package. Install it using pip:

   ```bash
   pip install qrcode[pil]
   ```

4. **Adjust the path to the `qrcode` module** (if necessary):
   
   If you have the `qrcode` module located in a custom directory, ensure that the path in `sys.path.append` matches the location of the module.

## Usage

1. **Run the Python script:**

   ```bash
   python qr_code_generator.py
   ```

2. **Follow the prompts:**
   - Enter the data you want to store in the QR code.
   - Provide a file name for the QR code image.
   - Decide if you want to display the generated QR code image.

3. **Generate additional QR codes:**
   - After generating one QR code, you will be prompted to generate another. Enter `Yes` to continue or `No` to exit.

## Example

```plaintext
Enter the data to be stored in the QR code: Hello, world!
Enter the file name for the QR code: hello_world
Do you want to display the QR code? (Yes/No): Yes
```

## Code Explanation

- **`qrcode`**: Generates the QR code.
- **`subprocess`**: Displays the QR code image using the default image viewer.
- **`sys.path.append`**: Includes the path to the custom `qrcode` module (if applicable).

## License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or support, please contact [fav.da24@gmail.com](mailto:fav.da24@gmail@example.com).
