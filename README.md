# 🧠 AI Brain Tumor Detector

This project is a Convolutional Neural Network (CNN) based Brain Tumor Detection and Classification web application built using Streamlit. The model detects and classifies MRI scan images into four categories:
- **No Tumor**
- **Glioma**
- **Meningioma**
- **Pituitary**

## 📂 Project Structure
Ensure your project folder (`4class.keras`) contains the following key files:
- `app.py`: The main Streamlit web application script.
- `requirements.txt`: The list of required Python dependencies.
- `config.json`: The Keras model configuration file.
- `model.weights.h5`: The trained model weights.
- `metadata.json`: Additional metadata for the model.

*(Note: The Streamlit app will automatically repackage the model components into a readable `.keras` archive when you run it for the first time).*

## 🚀 How to Run the Project Locally

### Step 1: Open Terminal / Command Prompt
Open your terminal or command prompt and navigate to the project directory:
```bash
cd "c:\Users\Saurav\OneDrive\Desktop\Final Year Project\4class.keras"
```

### Step 2: Create a Virtual Environment (Recommended)
It is highly recommended to use a virtual environment to avoid conflicts with global packages.
```bash
python -m venv venv
```

### Step 3: Activate the Virtual Environment
- **On Windows:**
  ```bash
  .\venv\Scripts\activate
  ```
- **On Mac/Linux:**
  ```bash
  source venv/bin/activate
  ```

### Step 4: Install Dependencies
Install all the required Python packages using `requirements.txt`:
```bash
pip install -r requirements.txt
```

### Step 5: Run the Streamlit App
Start the Streamlit development server:
```bash
streamlit run app.py
```

### Step 6: Access the Web App
The app should automatically open in your default web browser. If it doesn't, manually open your browser and navigate to:
**http://localhost:8501**

---

## 🐳 How to Run with Docker

### Option 1: Using Docker CLI
1. **Build the Docker Image:**
   ```bash
   docker build -t brain-tumor-detector .
   ```
2. **Run the Container:**
   ```bash
   docker run -p 8501:8501 brain-tumor-detector
   ```
3. Open your browser and navigate to **http://localhost:8501**.

### Option 2: Using Docker Compose
```bash
docker compose up --build
```

### Option 3: Using Docker Compose In Detatch Mode
```bash
docker compose up -d --build
```

### Stop Docker Containers Using Docker Compose
```bash
docker compose down
```

---
### 💡 How to Use
1. Once the web app opens, click on the **"Browse files"** button or drag and drop an MRI scan image (supported formats: JPG, JPEG, PNG).
2. The AI will instantly analyze the scan and automatically display the **Diagnosis Result** and **Confidence Level** without requiring any further clicks!
