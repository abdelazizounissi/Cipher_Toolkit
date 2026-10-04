# 🔐 Cipher Toolkit

A simple Flask web app that encrypts and decrypts text using two classic ciphers. Pick a cipher, choose an action, and see the result in your browser.

> ⚠️ Built for learning and demonstration only. Classical ciphers are **not** secure for real-world use.

<img width="1919" height="975" alt="Cipher Toolkit screenshot" src="https://github.com/user-attachments/assets/3f511501-704d-491d-97f3-7ac63d5b98b7" />

## ✨ Features

- **Two Classic Ciphers**:
  - Monoalphabetic substitution cipher (preserves letter case)
  - Caesar cipher (rotational shift from 1 to 25)
- **Encrypt or Decrypt**: Choose the action with one selection
- **Custom Caesar Shift**: Set any shift value between 1 and 25
- **Case and Symbol Preservation**: Uppercase and lowercase letters stay as they are, and non-letter characters are left unchanged
- **Local Web Interface**: Runs in your browser, nothing is sent to an outside server

## 📋 Requirements

- Python 3.8 or newer
- pip
- Flask (installed from `requirements.txt`)

## 🚀 Installation & Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/abdelazizounissi/Cipher_Toolkit.git
   cd Cipher_Toolkit
   ```

2. Create and activate a virtual environment:

   **Windows (PowerShell):**
   ```powershell
   python -m venv venv
   venv\Scripts\Activate.ps1
   ```

   **macOS / Linux:**
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the app:
   ```bash
   python app.py
   ```

5. Open your browser and go to:
   ```
   http://127.0.0.1:5000
   ```

## 🎯 How to Use

1. **Enter Text**: Type or paste the text you want to process
2. **Choose a Cipher**: Monoalphabetic or Caesar
3. **Choose an Action**: Encrypt or Decrypt
4. **Set the Shift** (Caesar only): Enter a value from 1 to 25
5. **Run**: Click **Run Cipher** to see the result

## ⚙️ How It Works

- **Server**: Flask receives the form submission (POST) and runs the chosen cipher on the server side
- **Monoalphabetic**: Each letter is replaced using a fixed substitution mapping. Letter case is preserved and non-letter characters are kept as they are
- **Caesar**: Each letter is shifted by the chosen amount. Case and non-letter characters are preserved

## 📁 Project Structure

```
Cipher_Toolkit/
├── app.py              Flask app and cipher logic
├── templates/          HTML templates
├── requirements.txt    Dependencies
├── LICENSE
└── README.md
```

## 🔒 Security Note

Monoalphabetic and Caesar ciphers are **not secure** for real-world use. They can be broken in seconds and exist here for teaching and demonstration only.

For real confidentiality needs, use a well-maintained cryptographic library, for example the `cryptography` package with AES-GCM. Never commit private keys or secrets to a repository.

## 🗺️ Future Improvements

- [ ] Add automated tests (pytest)
- [ ] Add stronger input validation
- [ ] Add CSRF protection (Flask-WTF)
- [ ] Add rate limiting before any public deployment
- [ ] Add more ciphers (for example Vigenère)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

Abdelaziz Ounissi

[LinkedIn](https://www.linkedin.com/in/abdelaziz-ounissi/) | [GitHub](https://github.com/abdelazizounissi)

© 2025 Abdelaziz Ounissi

## 🤝 Contributing

Feel free to fork this project and submit pull requests for any improvements!

## 📧 Support

If you encounter any issues or have suggestions, please open an issue on GitHub.
