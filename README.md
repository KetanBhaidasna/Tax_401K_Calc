# 2026 Tax Calculator

A comprehensive Python notebook for calculating federal income tax, FICA deductions, and optimizing 401(k) contributions for the 2026 tax year.

## Features

- **2026 Tax Calculations**: Uses official IRS tax brackets and standard deductions from Revenue Procedure 2025-32
- **Multiple Filing Statuses**: Supports single, married filing jointly, and head of household
- **401(k) Optimization**: 
  - Traditional (pre-tax) 401(k) contributions
  - Roth 401(k) (post-tax) contributions
- **FICA Calculations**: Accurate Social Security and Medicare tax deductions
- **Interactive Visualizations**:
  - Matplotlib charts for annual and monthly breakdowns
  - Interactive ECharts plots with linked tooltips
  - Visual comparison of take-home pay vs. contribution rates

## Requirements

```
numpy
matplotlib
```

Install dependencies:
```bash
pip install numpy matplotlib
```

## Usage

1. Open `Tax_calc.ipynb` in Jupyter Notebook or VS Code
2. Modify the input parameters in the first cell:
   ```python
   filing_status = 'single'  # Options: 'single', 'married_filing_jointly', 'head_of_household'
   state_of_residence = 'TX'
   gross_income = 68000
   k401_contrib = 0.20  # 20% traditional 401(k)
   roth_401k_contrib = 0.10  # 10% Roth 401(k)
   ```
3. Run all cells to see:
   - Monthly breakdown (take-home pay, tax, 401(k), Roth 401(k))
   - Annual summary
   - Optimization charts showing the impact of different contribution rates

## Data Sources

- **Tax Brackets & Standard Deductions**: [IRS Revenue Procedure 2025-32](https://www.irs.gov/newsroom/irs-releases-tax-inflation-adjustments-for-tax-year-2026-including-amendments-from-the-one-big-beautiful-bill)
- **FICA Wage Base**: Social Security Administration (verify annually at [SSA.gov](https://www.ssa.gov/news/press/))

## Important Notes

⚠️ **Disclaimer**: This calculator is for educational and planning purposes only. It does not account for:
- State and local taxes
- Additional Medicare tax (0.9% on high earners)
- Net Investment Income Tax
- Tax credits and deductions beyond the standard deduction
- HSA, FSA, or other pre-tax benefits

Always consult with a qualified tax professional for personalized advice.

## Files

- `Tax_calc.ipynb` - Main calculator notebook
- `Tax_calc_rebuilt.ipynb` - Alternative version with similar functionality
- `*.html` - Generated ECharts visualization files

## Output Examples

The calculator generates:
1. **Monthly Breakdown**:
   - Monthly Take-Home Pay
   - Monthly Federal Tax
   - Monthly Traditional 401(k) Contribution
   - Monthly Roth 401(k) Contribution

2. **Interactive Charts**:
   - Annual and monthly comparisons
   - Impact of varying 401(k) contribution rates (0-20%)
   - Net income, taxes, FICA, and retirement contributions

## License

MIT License - See LICENSE file for details

## Contributing

Contributions are welcome! Please ensure that:
- Tax values are updated annually with official IRS publications
- All calculations are documented and sourced
- Code follows PEP 8 style guidelines

## Changelog

### 2026 Tax Year (January 2026)
- Updated to official 2026 IRS tax brackets and standard deductions
- Added Roth 401(k) contribution tracking
- Implemented percentage-based contribution inputs
- Enhanced visualizations with dual annual/monthly charts
- Added source citations for all tax values
