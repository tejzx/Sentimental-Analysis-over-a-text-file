# Text Emotion Analysis
This repository contains a Python script for performing emotion analysis on a text file. The script processes textual data to identify emotions and visualize the results using a bar chart.

## How It Works

1. **Input**: 
   - Reads a text file (`read.txt`) containing the input text for analysis.
   - Reads an emotion mapping file (`emotions.txt`) containing word-to-emotion mappings.

2. **Text Preprocessing**:
   - Converts all text to lowercase.
   - Removes punctuation.
   - Tokenizes text into individual words.
   - Removes stop words using a predefined list of common stop words.

3. **Emotion Detection**:
   - Compares each word in the processed text against the `emotions.txt` file.
   - Matches are used to build a list of emotions corresponding to the text.

4. **Visualization**:
   - Counts the frequency of each detected emotion.
   - Displays a bar chart showing the distribution of emotions.
   - Saves the bar chart as `graph.png`.

## Requirements

- Python 3.7+
- Required Python Libraries: `matplotlib`

Install the necessary dependencies using:
```bash
pip install matplotlib
```

## Files in the Repository

1. `main.py`: The main script for text emotion analysis.
2. `read.txt`: Input text file to be analyzed.
3. `emotions.txt`: File containing word-to-emotion mappings.

## Usage

1. **Prepare Input Files**:
   - Place the text to be analyzed in `read.txt`.
   - Ensure `emotions.txt` contains valid word-to-emotion mappings in the format:
     ```
     word:emotion
     ```

2. **Run the Script**:
   Execute the script:
   ```bash
   python main.py
   ```

3. **View Results**:
   - The script outputs the detected emotions and their frequencies to the console.
   - A bar chart visualizing the emotion distribution is saved as `graph.png` and displayed.

## Example

### Sample Input (`read.txt`):
```
I am so happy and excited to see you here! However, I feel a bit nervous about the results.
```

### Sample Emotion Mapping (`emotions.txt`):
```
happy:joy
excited:joy
nervous:fear
```

### Output:
Console Output:
```
['joy', 'joy', 'fear']
Counter({'joy': 2, 'fear': 1})
```

Bar Chart:
- A bar chart showing `joy` with a count of 2 and `fear` with a count of 1.

## License
This project is licensed under the MIT License.

## Acknowledgments
Thanks to the creators of the emotion mapping dataset for providing a valuable resource for emotion analysis.

