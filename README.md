# WhatsApp Chat Analyzer

A Python-based WhatsApp chat analysis tool that provides insights and visualizations from WhatsApp chat exports. The tool analyzes chat patterns, user activity, word frequencies, and emoji usage through an interactive Gradio interface.

## Features

- **Most Active Senders Analysis**: Visualizes the top 10 most active participants in the chat
- **Message Timeline**: Tracks message frequency over time with monthly aggregation
- **Active Hours Analysis**: Shows the most active hours of conversation
- **Word Cloud Generation**: Creates word clouds from chat messages with stopword filtering
- **Emoji Analysis**: Displays the most frequently used emojis
- **Flexible Analysis Scope**: Analyze either the entire chat or specific sender's messages
- **Interactive Web Interface**: Easy-to-use Gradio web interface for analysis


## Required Libraries
- pandas: Data processing and analysis
- wordcloud: Word cloud visualization
- emoji: Emoji analysis
- matplotlib: Data visualization
- seaborn: Enhanced data visualization
- nltk: Natural language processing
- gradio: Web interface creation
- urlextract: URL extraction from text
  
## Prerequisites
```bash
pip install pandas wordcloud emoji matplotlib seaborn nltk gradio urlextract
```
## Usage
**1. Export your WhatsApp chat:**  
- Open WhatsApp chat
- Click on three dots (⋮) > More > Export chat
- Choose 'Without Media'
- Save the .txt file
  
**2.Run the notebook :**
  Run the notebook and wait for it to deploy on gradio.  
  
**3.Using the Web Interface:**
<img width="818" alt="Demo" src="https://github.com/user-attachments/assets/f9915219-b6ef-4bfc-ac88-fa2b170a7be5" />

- Upload your chat .txt file
- Select analysis type:
   - Most Active Senders
   - Messages Over Time
   - Active Hours
   - Common Words Word Cloud
   - Emoji Analysis


- Choose analysis scope (Overall/Specific Sender)
- Click "Analyze" to generate visualizations

## Features in Detail
### Chat Parsing
- Handles date and time formats from WhatsApp exports
- Removes system messages
- Processes message continuations correctly
- Extracts emojis and cleans text
  
### Text Processing
- Custom stopword removal (English + Hinglish)
- Message cleaning and preprocessing
- Emoji extraction and analysis
- Time-based analysis (hourly, daily, monthly patterns)

### Visualization Types
**Activity Analysis**  
- Bar charts for sender activity
  <img width="718" alt="most active senders" src="https://github.com/user-attachments/assets/bd9ce6e4-5d5a-42fa-9a84-2ff3670fe1e0" />

- Time series plots for message frequency
  <img width="863" alt="messageovertime" src="https://github.com/user-attachments/assets/f8e1a76d-56ea-4ed6-94a0-581f57dbe85f" />

- Hourly activity heatmaps
<img width="599" alt="Hourly actiity" src="https://github.com/user-attachments/assets/b7aa632b-9de5-4adb-8816-58821cc7f8a2" />

### Content Analysis
- Word clouds for common terms
  <img width="803" alt="wordcloud" src="https://github.com/user-attachments/assets/52e19057-29c2-4e35-a272-4f186a2a95bd" />

- Emoji frequency charts
 <img width="770" alt="most common emojis" src="https://github.com/user-attachments/assets/2205a882-e3f0-4338-82ed-7323b55a9756" />

- Message length statistics

### Data Privacy
- All processing is done locally
- No data is stored or transmitted
- Compatible with end-to-end encrypted chat exports
  
