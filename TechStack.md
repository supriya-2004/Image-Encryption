# ⚙️ Technology Stack  

This project utilizes various technologies and libraries to perform image encryption and decryption using pixel manipulation. Below is a detailed breakdown of the tools and technologies used.  

## 🖥️ Programming Language  
- **Python** 🐍 → Used for scripting and handling image processing operations efficiently.  

## 📦 Libraries & Dependencies  
- **NumPy** 🔢 → Used for numerical operations, handling image matrices, and performing bitwise XOR operations for encryption and decryption.  
- **Pillow (PIL)** 🖼️ → Used for opening, processing, and saving images in different formats.  

## 🔢 How It Works  
🔹 Loads the input image and converts it into a NumPy array.  
🔹 Generates a random key of the same dimensions as the image.  
🔹 Uses bitwise XOR (`np.bitwise_xor`) for encryption and decryption.  
🔹 Saves the encrypted and decrypted images.  

## 📊 Algorithm Overview  
1️⃣ **Image Conversion** → The image is converted into an array for pixel-level operations.  
2️⃣ **Key Generation** → A random matrix (same size as the image) acts as the encryption key.  
3️⃣ **Encryption Process** → The key is XOR-ed with the image matrix, altering pixel values.  
4️⃣ **Decryption Process** → The same key is XOR-ed again to retrieve the original image.  

## 🏗️ Elements Used 
### 🔹 PIL (Pillow)
Used to open, process, and save images in various formats.

### 🔹 NumPy
Used for efficient numerical computations, handling image data as arrays.

### 🔹 Image Opening (`Image.open()`)
Loads the image into memory.

### 🔹 Image to Array (`np.array(img)`)
Converts the image into a numerical array for manipulation.

### 🔹 Bitwise XOR (`np.bitwise_xor(img_array, key) `)
Encrypts the image by modifying pixel values.

### 🔹 Array to Image (`Image.fromarray()`)
Converts the modified array back into an image.

### 🔹 Save Image (`.save(output_image_path)`)
Stores the encrypted image file.

### 🔹 Reversing XOR (`np.bitwise_xor(encrypted_array, key)`)
XOR-ing the encrypted data again with the same key restores the original image.

### 🔹 Array to Image (`Image.fromarray()`)
Converts decrypted data back to an image.

### 🔹 Save Image (`.save(output_image_path)`)
Stores the decrypted image.

### 🔹 Check if script is running directly (`if __name__ == "__main__":`)
Ensures the script runs only when executed directly, not when imported as a module.

### 🔹 Open the Input Image (`Image.open()`)
Loads the original image.

### 🔹 Get Image Dimensions (`img.size`)
Extracts width and height.

### 🔹 Generate Random Key (`np.random.randint()`)
Creates a key matching the image size (height, width, 3 for RGB).

### 🔹 Encrypt Image (`encrypt_image()`)
Encrypts the image and saves it.

### 🔹 Decrypt Image (`decrypt_image()`)
Restores the original image.

## 🔚 Conclusion
This project demonstrates a basic image encryption technique using NumPy and PIL. While it provides fundamental image security through pixel-level encryption, it is not suitable for high-security applications. For real-world scenarios, implementing cryptographic methods such as AES or RSA is recommended. 🚀

