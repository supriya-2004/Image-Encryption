# 🖼️ Image Encryption Tool

## 🔒 Problem Statement  
Develop a simple image encryption tool using pixel manipulation. The program should allow users to encrypt and decrypt images by modifying pixel values through operations like swapping pixel values or applying basic mathematical transformations to each pixel.

## ✨ Features  
✅ Encrypts images by altering pixel values.  
✅ Decrypts images back to their original form.  
✅ Uses pixel swapping and mathematical operations for encryption.  
✅ Ensures image security through pixel-level transformations.  

## 🚀 Getting Started  

### 📌 Prerequisites  
Ensure you have Python installed along with the required dependencies. Install the necessary libraries using:  

```bash
pip install pillow numpy
```
## 🛠️ How It Works  
🔹 Loads the input image and converts it into a NumPy array.  
🔹 Generates a random key of the same dimensions as the image.  
🔹 Uses bitwise XOR (`np.bitwise_xor`) for encryption and decryption.  
🔹 Saves the encrypted and decrypted images.  

## 📌 Notes  
⚠️ The encryption method is simple and does not provide high security.  
⚠️ The same key is required for decryption, so store it securely.  
⚠️ For stronger encryption, consider advanced cryptographic techniques.  

## 🔚 Conclusion  
This project demonstrates a basic image encryption technique using NumPy and PIL. While it offers a simple way to secure images, it lacks advanced security measures required for real-world applications. For enhanced security, integrating robust cryptographic algorithms like AES or RSA is recommended. 🚀  
