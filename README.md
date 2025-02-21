🔒 Secure Data Hiding in Images using Steganography
A Python-based steganography project using OpenCV to securely hide and retrieve secret messages inside images.

📌 Overview
Steganography is the practice of hiding information within digital media. This project implements image steganography using Python and OpenCV, allowing users to embed and extract messages within an image securely. The message is hidden within the RGB pixel values, ensuring that the embedded text is imperceptible to the human eye.

🚀 Features
✔ Secure Data Hiding – Encodes text messages into image pixels without visible distortion.
✔ Passcode Protection – Ensures only authorized users can retrieve the hidden message.
✔ Lightweight & Efficient – Uses Python and OpenCV for direct pixel manipulation.
✔ Cross-Platform Compatibility – Runs on Windows, macOS, and Linux without additional dependencies.
✔ No External Storage – The message remains inside the image, making it untraceable.

🛠️ Installation
📌 Prerequisites
Ensure you have Python 3.x installed on your system. If not, download it from Python.org.

📌 Install Required Libraries
Run the following command to install OpenCV:

sh
Copy
Edit
pip install opencv-python
💡 How It Works
🔑 Encryption Process
The user selects an image and enters a secret message and passcode.
The message characters are converted to their ASCII values and embedded into the RGB pixel values.
The modified image is saved as encryptedImage.jpg, containing the hidden message.
🔓 Decryption Process
The user enters the correct passcode to extract the hidden message.
If the passcode is correct, the original hidden message is retrieved from the image pixels.
If the passcode is incorrect, access is denied.
📜 Usage
🔹 Run the Script
Execute the following command:

sh
Copy
Edit
python steganography.py
🔹 Encryption: Hiding a Message
1️⃣ The script prompts the user to enter a secret message.
2️⃣ The user provides a passcode to encrypt the message.
3️⃣ The message is embedded in the image and saved as encryptedImage.jpg.
4️⃣ The encrypted image is displayed.

🔹 Decryption: Retrieving the Message
1️⃣ The user runs the script and enters the correct passcode.
2️⃣ If the passcode matches, the hidden message is revealed.
3️⃣ If the passcode is incorrect, "Unauthorized Access!" is displayed.

📷 Example
Encryption Process
yaml
Copy
Edit
Enter secret message: Hello, World!
Enter a passcode: secure123
✔️ Image saved as encryptedImage.jpg

Decryption Process
yaml
Copy
Edit
Enter passcode for decryption: secure123
Decrypted message: Hello, World!
🔴 If an incorrect passcode is entered, access is denied!

🔮 Future Enhancements
✅ AES/RSA Encryption – Encrypt the message before embedding for added security.
✅ Steganography in Videos – Extend the project to hide messages in video frames.
✅ GUI Development – Implement a Tkinter or PyQt-based user interface for ease of use.
✅ Multi-Layer Security – Introduce multiple security layers for enhanced protection.
✅ Mobile App Integration – Develop an Android/iOS version for secure steganography on mobile devices.

