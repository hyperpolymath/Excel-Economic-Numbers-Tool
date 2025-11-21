# Excel Economic Number Tool

## Project Overview

This project provides a tool for working with economic numbers in Excel format. It's designed to handle, format, and process economic data such as GDP, inflation rates, interest rates, and other financial/economic indicators.

## Purpose

The Excel Economic Number Tool aims to:
- Parse and validate economic data from Excel files
- Format large numbers according to economic conventions (millions, billions, trillions)
- Handle various economic data types (percentages, currencies, indices)
- Provide utilities for common economic calculations
- Support data transformation and export

## Technology Stack

### Expected Technologies
- **Language**: Python/JavaScript/TypeScript (to be determined)
- **Excel Processing**: Libraries for reading/writing Excel files (e.g., openpyxl, pandas, ExcelJS)
- **Data Processing**: Numerical computation libraries
- **Testing**: Unit and integration testing frameworks

## Project Structure

```
excel-economic-number-tool/
├── src/                    # Source code
│   ├── parsers/           # Excel file parsers
│   ├── formatters/        # Number formatting utilities
│   ├── validators/        # Data validation
│   └── utils/             # Helper functions
├── tests/                 # Test files
├── examples/              # Example usage and sample files
├── docs/                  # Documentation
└── data/                  # Sample economic data files
```

## Key Features

### 1. Number Formatting
- Format numbers in thousands (K), millions (M), billions (B), trillions (T)
- Support for different international number formats
- Currency formatting with multiple currency support
- Percentage formatting with configurable precision

### 2. Data Processing
- Parse Excel sheets containing economic indicators
- Validate data types and ranges
- Handle missing or invalid data
- Support for time-series economic data

### 3. Economic Calculations
- Growth rate calculations (YoY, MoM, QoQ)
- Index calculations and rebasing
- Moving averages and trends
- Inflation adjustments

## Development Guidelines

### Code Style
- Follow language-specific best practices
- Use meaningful variable names that reflect economic terminology
- Comment complex calculations with economic context
- Keep functions focused and single-purpose

### Testing
- Write unit tests for all formatting and calculation functions
- Include integration tests for Excel file processing
- Test edge cases: zero values, negative numbers, very large/small numbers
- Validate with real economic data samples

### Data Handling
- Always validate input data before processing
- Handle errors gracefully with informative messages
- Support common economic data formats (CSV, XLSX, JSON)
- Preserve data precision for financial calculations

### Performance Considerations
- Optimize for large Excel files (thousands of rows)
- Implement streaming for very large datasets
- Cache frequently used calculations
- Profile and optimize bottlenecks

## Economic Data Conventions

### Number Formatting Standards
- GDP, Revenue, Expenditure: Typically in millions or billions
- Interest Rates, Inflation: Percentage format (e.g., 2.5%)
- Exchange Rates: High precision decimal (4-6 decimal places)
- Index Values: Usually base 100 or base value specified

### Common Economic Indicators
- GDP (Gross Domestic Product)
- CPI (Consumer Price Index)
- Unemployment Rate
- Interest Rates (Federal Funds Rate, LIBOR, etc.)
- Exchange Rates
- Trade Balance
- Industrial Production Index

## Usage Examples

### Basic Number Formatting
```python
# Example: Format a large number
value = 1500000000
formatted = format_economic_number(value)  # "1.5B"
```

### Processing Excel Files
```python
# Example: Load and process economic data
data = load_excel("economic_indicators.xlsx")
formatted_data = format_all_numbers(data)
export_to_excel(formatted_data, "output.xlsx")
```

## Installation & Setup

(To be added based on chosen technology stack)

## API Reference

(To be added as features are implemented)

## Contributing

When contributing to this project:
1. Understand economic data conventions
2. Test with realistic economic datasets
3. Ensure calculations are numerically stable
4. Document any assumptions about data format
5. Follow existing code style and patterns

## Known Limitations

(To be documented as project develops)

## Future Enhancements

Potential features for future development:
- Web interface for uploading and processing Excel files
- API endpoints for programmatic access
- Support for additional economic data sources
- Data visualization capabilities
- Automated report generation
- Multi-language support for international formats

## Resources

### Economic Data Sources
- World Bank Open Data
- IMF Data
- OECD Statistics
- Federal Reserve Economic Data (FRED)
- BLS (Bureau of Labor Statistics)

### Related Standards
- ISO 4217 (Currency Codes)
- ISO 3166 (Country Codes)
- SNA (System of National Accounts)

## License

(To be determined)

## Contact

Repository: Hyperpolymath/excel-economic-number-tool-
