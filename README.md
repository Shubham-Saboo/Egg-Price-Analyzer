# 🥚 Egg Price Analyzer

![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
![OpenAI](https://img.shields.io/badge/OpenAI-Agents%20SDK-green.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-UI-red.svg)

An intelligent tool that helps users find the cheapest egg prices in their city by scraping retail websites and providing detailed price comparisons.

## 🚀 Features

- 🔍 **Targeted Price Research**: Searches websites like Walmart, Target, DoorDash, and local grocers for real-time egg prices
- 📊 **Detailed Analysis**: Compares prices across different stores and egg types (regular, organic, free-range)
- 💰 **Focus on Value**: Identifies the absolute cheapest options available in a specified city
- 📝 **Comprehensive Reporting**: Generates a markdown report with price breakdowns and shopping recommendations
- 📉 **Data Visualization**: Displays collected prices in an interactive table with comparison charts

## 🛠️ Tech Stack

- **OpenAI Agents SDK**: Orchestrates the research process using specialized AI agents
  - Master Agent: Plans the research approach
  - Price Research Agent: Collects price data from retail websites
  - Analysis Agent: Interprets data and generates insights
- **Streamlit**: Powers the interactive web interface
- **Python**: Core programming language
- **Pydantic**: Data validation and settings management
- **Pandas**: Data manipulation and analysis
- **Asyncio**: Asynchronous I/O management
- **dotenv**: Environment variable management

## ⚙️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/egg-price-researcher.git
   cd egg-price-researcher
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the project root with your OpenAI API key:
   ```
   OPENAI_API_KEY=your_openai_api_key_here
   ```

## 🚀 Usage

Run the Streamlit app:
```bash
streamlit run app.py
```

This will launch the web interface in your default browser. From there:

1. Enter a city in the input field (e.g., "Seattle, WA")
2. Click "Start Research" to begin the automated price search
3. Watch as the agents collect and analyze egg prices in real-time
4. Review the comprehensive price report on the "Final Report" tab
5. Explore the raw data on the "Price Data" tab
6. Download the report or raw data as needed

## 📋 Requirements

Dependencies are listed in `requirements.txt`, but the major ones include:

```
streamlit>=1.30.0
openai>=1.20.0
pandas>=2.0.0
pydantic>=2.0.0
python-dotenv>=1.0.0
```

## 🧩 Project Structure

```
egg-price-researcher/
├── app.py             # Main application file
├── agents.py          # Agent definitions and tools
├── requirements.txt   # Project dependencies
├── .env               # Environment variables (not in repo)
└── README.md          # This file
```

## 🔒 Privacy & Usage Notes

- This application performs web searches on your behalf
- No personal data is stored beyond the current session
- The egg price data is ephemeral and not stored in any database
- Be mindful of rate limits on the OpenAI API when running extensive research

## 📝 License

MIT

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
