# Text Emotion Analysis

## 📌 Overview
This project performs **emotion analysis** on a given text file, identifying and visualizing emotions present in the text. The script processes textual data, detects emotions using predefined word mappings, and presents the results in a bar chart.

## 🚀 Features
- Reads input text from a file.
- Processes and cleans text (lowercasing, punctuation removal, tokenization).
- Maps words to emotions using a predefined dictionary.
- Counts and visualizes detected emotions.
- Saves results as a bar chart.

## 🛠️ Installation
### Prerequisites
- **Python 3.7+**
- Required libraries:
  ```bash
  pip install matplotlib
  ```

## 📂 Project Structure
```
📁 TextEmotionAnalysis
│── 📄 main.py            # Main script for emotion analysis
│── 📄 read.txt           # Input text file
│── 📄 emotions.txt       # Word-to-emotion mapping
│── 📄 graph.png          # Output visualization (generated)
```

## 🔧 How It Works
1. **Preprocessing:**
   - Converts text to lowercase.
   - Removes punctuation.
   - Tokenizes words.
2. **Emotion Detection:**
   - Compares words with `emotions.txt`.
   - Identifies and counts emotions.
3. **Visualization:**
   - Generates a bar chart.
   - Saves output as `graph.png`.

## 🏃 Usage
### 1️⃣ Prepare Input Files
- **`read.txt`**: Add text for analysis.
- **`emotions.txt`**: Define word-emotion mappings (`word:emotion`).

### 2️⃣ Run the Script
Execute the script using:
```bash
python main.py
```

### 3️⃣ View Results
- Console output shows detected emotions and their count.
- The bar chart (`graph.png`) visualizes the emotion distribution.

## 📝 Example
### **Sample Input (`read.txt`)**:
```
I am so happy and excited to see you here! However, I feel a bit nervous about the results.
```

### **Sample Mapping (`emotions.txt`)**:
```
happy:joy
excited:joy
nervous:fear
```

### **Output**:
Console Output:
```
['joy', 'joy', 'fear']
Counter({'joy': 2, 'fear': 1})
```
Bar Chart:
- Shows `joy: 2`, `fear: 1`.

## 📜 License
This project is licensed under the **MIT License**.

## 🙌 Acknowledgments
Special thanks to the creators of emotion mapping datasets for their contributions to NLP research.

---
💡 **Contributions Welcome!** Feel free to submit issues or feature requests. 🚀
