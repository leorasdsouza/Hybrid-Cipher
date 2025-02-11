# Hybrid Cipher

This program implements a **128-bit hybrid cipher** that combines **AES (substitution)** and **block-level transposition** for secure encryption.

---

## Features
- 128-bit Encryption Strength: Uses AES for strong substitution.
- Block-level Transposition: Rearranges ciphertext blocks for added security.
- Supports Any Plaintext: Encrypts and decrypts text of any length.
- Preserves Data Integrity: Ensures the decrypted text matches the original plaintext.
  
---

## How It Works

### Substitution (AES Encryption)
- The plaintext is encrypted using AES in CBC mode with a 128-bit key.  
- AES provides strong confusion and diffusion, making the ciphertext resistant to cryptanalysis.

### Transposition (Block-level Permutation)
- The AES ciphertext is divided into 128-bit blocks.  
- The blocks are rearranged based on a user-defined transposition key.  

### Decryption
- The transposition is reversed to restore the original block order.  
- The rearranged ciphertext is decrypted using AES to recover the plaintext.  

## How to Run
### **Option 1: Run using Google Colab
1. Open the notebook in Google Colab:
   - Click on the `hybrid_cipher.ipynb` file in the repository.
   - Click the **Open in Colab** button.

2. Run the notebook:
   - Execute the notebook to see the hybrid cipher in action.
#### **Option 2: Run Locally**
1. Download the script `HybridCipher.py` from this repository.
2. Open a terminal or command prompt.
3. Run the following command:
   ```bash
   python HybridCipher.py

---

### Sample Output
![image](https://github.com/user-attachments/assets/b458318f-8aa2-4673-bb2a-ea274c87748c)

