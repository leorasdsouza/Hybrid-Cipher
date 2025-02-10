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

---
## Repository Structure

- `hybrid_cipher.ipynb`: Google Colab notebook containing the implementation and examples.
- `ins_assignment_hybrid_cipher.pdf`: Detailed report explaining the cipher design, examples, and security evaluation.

---

## How to Run

1. Open the notebook in Google Colab:
   - Click on the `hybrid_cipher.ipynb` file in the repository.
   - Click the **Open in Colab** button.

2. Run the notebook:
   - Execute the notebook to see the hybrid cipher in action.

---

## Detailed Report

The detailed report is available as a PDF file (`ins_assignment_hybrid_cipher.pdf`). It includes:
1. Cipher design process.
2. Encryption and decryption examples.
3. Security evaluation of the hybrid cipher.
4. Mathematical formulation of the cipher design process.

[View the Report](ins_assignment_hybrid_cipher.pdf)

---

### Sample Output
![image](https://github.com/user-attachments/assets/b458318f-8aa2-4673-bb2a-ea274c87748c)


## **License**

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
