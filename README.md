# BCGXGENAI_simple_financial_chatbot_app



# Financial Query Bot

A Python-based chatbot that provides instant financial insights from company financial data. This tool processes structured financial data and answers natural language queries about key business metrics.

## Features

- **Interactive Chat Interface**: Natural conversation-based query system
- **Key Financial Metrics**: Total revenue, net income, revenue trends, and company performance
- **Data Transformation**: Automatically converts financial data from long to wide format for analysis
- **Predefined Queries**: Handles common financial questions with accurate responses

## Supported Queries

- "What is the total revenue?"
- "What is the total net income?" 
- "What is the average revenue?"
- "How has net income changed over the last year?"
- "Which company has the highest revenue?"

## Installation

1. Clone or download this repository
2. Ensure you have Python installed
3. Install required dependencies:

```bash
pip install pandas
```

## Usage

1. **Prepare Your Data**: 
   - Format your financial data as a CSV file with columns: `Company`, `Year`, `Financial_Term`, `Value`
   - Name your file `company_financial_data.csv` or update the filename in the code

2. **Run the Application**:
```bash
python financial_chatbot.py
```

3. **Interact with the Bot**:
   - Type financial questions in natural language
   - Use `help` to see available commands
   - Use `quit`, `exit`, or `bye` to end the session

## Data Format Requirements

Your CSV file should follow this structure:

| Company | Year | Financial_Term | Value |
|---------|------|----------------|-------|
| Company A | 2023 | Total_Revenue | 1000000 |
| Company A | 2023 | Net_Income | 150000 |
| Company B | 2023 | Total_Revenue | 750000 |

## Code Structure

- **Data Loading & Transformation**: Reads CSV and pivots data for analysis
- **Metric Calculations**: Pre-computes key financial indicators
- **Chatbot Engine**: Processes user queries and returns relevant insights
- **Interactive Loop**: Maintains conversation until user exits

## Example Output

```
Financial Query Bot activated! Type 'help' for options or 'quit' to exit.

Ask a financial question: what is the total revenue
The total revenue is 15,750,000.00.

Ask a financial question: which company has the highest revenue
The company with the highest total revenue is TechCorp Inc.
```

## Customization

To add new query capabilities:
1. Add the calculation logic in the data processing section
2. Extend the `simple_chatbot` function with new conditional statements
3. Update the help menu to reflect new capabilities

## Limitations

- Currently supports only predefined queries
- Requires specific data format for processing
- Basic natural language processing (exact match based)

## Future Enhancements

- Integration with more advanced NLP libraries
- Support for additional financial metrics
- Database connectivity for real-time data
- Visualization capabilities
- Web interface version

## License

This project is provided for educational and demonstration purposes.

---

This README provides clear documentation while maintaining a professional tone suitable for sharing on platforms like GitHub or with colleagues.
