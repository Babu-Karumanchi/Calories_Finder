

# Gemini Health App

## Overview

The **Gemini Health App** is an AI-powered health management tool that allows users to analyze food images and get detailed nutritional information. It uses the Google Gemini Pro Vision API for image recognition and calorie calculation, providing a simple and intuitive interface via Streamlit.

## Features

- **Food Image Analysis**: Upload a food image, and the app identifies the items and calculates their calorie content.
- **Detailed Reports**: Get a detailed breakdown of calories for each food item, along with the total calorie count.
- **Interactive Interface**: Powered by Streamlit, the app offers a user-friendly experience for image uploads and viewing results.

## Technologies Used

- **Python**
- **Streamlit**: For creating a web-based user interface.
- **Google Gemini Pro Vision API**: For AI-driven image recognition and analysis.
- **Pillow (PIL)**: For handling image processing.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/travel-planner.git
   cd travel-planner
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up your API keys:
   - Create a `.env` file in the root directory of the project:
   - Add your Google API key to the `.env` file in the following format:
     ```
     GOOGLE_API_KEY=your_api_key_here
     ```
   - Replace `your_api_key_here` with your actual Google API key.

4. Run the application:
   ```bash
   streamlit run health.py
   ```

5. Open the app in your browser at `http://localhost:8501`.

## Usage

1. **Upload an Image**: Choose a `.jpg`, `.jpeg`, or `.png` image of food items.
2. **Enter a Custom Prompt (Optional)**: Provide additional instructions in the input box.
3. **Analyze**: Click the **"Tell me the total calories"** button to process the image and display results.

## Input and Output

### Input
- **Image**: Upload a clear picture of your food items.

### Output
- **Food Item Details**: Calorie information for each identified food item.
  
### Example
#### Input:
- **Image**: A plate of spaghetti, garlic bread, and salad.

#### Output:
```
1. Spaghetti - 400 calories
2. Garlic Bread - 150 calories
3. Salad - 50 calories

```

## Directory Structure

```
.
├── health.py         # Main application file
├── requirements.txt  # List of dependencies
├── .env              # Environment file for API keys
└── README.md         # Project documentation
```
