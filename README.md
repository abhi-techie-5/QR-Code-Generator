# QR-Code-Generator
📱 URL to QR Code Generator
A simple Python script that converts any URL into a QR code image and saves it as a PNG file.

FEATURES

Convert any URL or link into a QR code
Save the generated QR code as a PNG image
Auto-adds .png extension if not provided by the user
Lightweight and easy to use


TECH STACK
Language: Python 3
Library: qrcode


USAGE
Run the script:
python main.py
Example Interaction:
Enter your url: https://www.github.com
Filename you want to save it as: my_qrcode
Output: my_qrcode.png (saved in the current directory)

PROJECT STRUCTURE
url-to-qrcode/
├── main.py      -> Main Python script
└── README.md    -> Project documentation

HOW IT WORKS

The user enters a URL to convert.
The user provides a filename to save the QR code.
If the filename doesn't end with .png, it is added automatically.
The qrcode library generates the QR code and saves it as a PNG image.


REQUIREMENTS
qrcode[pil]
Install via:
pip install qrcode[pil]
Note: The [pil] extra is required for image saving support (uses Pillow internally).

CUSTOMIZATION
You can extend the script to customize QR code properties like size, color, or error correction level using the qrcode library's advanced options:
qr = qrcode.QRCode(
version=1,
error_correction=qrcode.constants.ERROR_CORRECT_H,
box_size=10,
border=4,
)
Author

Created by Abhishek Suman

License

This project is open-source and free to use for learning purposes.
