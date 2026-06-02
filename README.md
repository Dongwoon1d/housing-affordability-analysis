# Housing Affordability Analysis Across U.S. Metro Areas

## Overview

This project analyzes housing affordability across selected major U.S. Metro Areas using data from the U.S. Census ACS 5-Year dataset.

The goal is to compare rental housing burden by looking at both median household income and median gross rent. Instead of analyzing rent prices alone, this project uses the rent-to-income ratio to understand how much of a household's monthly income is spent on rent.

## Project Question

Which major U.S. Metro Areas have the highest rental housing burden when rent is compared to household income?

Additional questions:

- Are high-rent Metro Areas always the least affordable?
- Do higher-income Metro Areas have lower rent burden?
- How does rent-to-income ratio differ across major rental markets?

## Data Source

The data comes from the U.S. Census ACS 5-Year dataset.

Main variables used:

- `B19013_001E`: Median Household Income
- `B25064_001E`: Median Gross Rent

The analysis uses Metro Area-level data from the Census API.

## Methodology

The project calculates the following metrics:

```text
Monthly Income = Median Household Income / 12
Rent-to-Income Ratio = Median Gross Rent / Monthly Income
```

The rent-to-income ratio is used to compare rental housing burden across Metro Areas.

## Key Findings

- Among the selected 29 Metro Areas, Miami-Fort Lauderdale-West Palm Beach had the highest rent-to-income ratio.

- Several Florida and California Metro Areas appeared among the highest rent-burden markets in the selected sample.

- High rent alone does not fully explain housing affordability.

- Comparing rent with income provides a clearer view of rental market pressure.

- None of the selected 29 Metro Areas exceeded the 30% cost-burden threshold when using median household income and median gross rent.

- Median-based analysis may hide the housing burden experienced by lower-income renters.

## Limitations

This project uses median household income and median gross rent, which provide a useful overall picture of each Metro Area.

However, median values do not fully represent all renter experiences. Lower-income renters, students, and households with unstable income may face much higher housing burden than the median numbers suggest.

This project also focuses on 29 selected Metro Areas, so the results should not be interpreted as a full ranking of all U.S. housing markets.

## Future Improvements

Future versions of this project could include:

- More Metro Areas

- Poverty rate

- Median home value

- Renter household income instead of general household income

- Year-over-year affordability trends

- Map-based visualization

- A focused analysis on Wisconsin or Madison

## Tools Used

- Python

- Pandas

- Requests

- Matplotlib

- U.S. Census ACS API
