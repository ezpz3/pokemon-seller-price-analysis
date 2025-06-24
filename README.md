# Pokémon Listing Price Analysis

This project analyzes eBay listings for a specific Pokémon item — the Prismatic Evolutions Super Premium Collection — to determine whether seller status affects listing prices.

## Summary

Using Python, I compared listing prices using two indicators of seller status:

- Listings labeled as **Top-Rated Plus Items** vs. those that were not.

- Sellers labeled as **Top Sellers** vs. those that were not.

For both groups, I computed summary statistics (mean, median, min, and max) and visualized the distributions:

- **Boxplot** for Top-Rated Plus vs. Non-Top-Rated Plus items.

- **KDE plot** for Top Sellers vs. Non-Top Sellers.

Finally, I conducted a **Mann-Whitney U test** to check for statistical significance. The results suggest no significant difference in listing prices based on seller status.

## Seller Status Definitions

**Top-Rated Plus Item**: An official eBay listing badge for items that meet strict criteria:
- A minimum 30-day money-back return policy
- Shipping within 1 business day (with tracking)
- Sold by an experienced seller with the highest buyer ratings

**Top Seller** (custom-defined): In this project, a seller is classified as a Top Seller if they meet both of the following criteria:
- Feedback percentage ≥ 99%
- Feedback score ≥ 100

## Tools
- Python
- JupyterLab
- pandas, numpy, matplotlib, seaborn, scipy
- eBay Browse API

## Findings

- No statistically significant price difference between Top Sellers and Non-Top Sellers.
- No statistically significant price difference between Top-Rated Plus listings and others.

## How to Run
1. Clone the repository.
2. Open `pokemon price analysis.ipynb` in Jupyter.
3. Provide your own eBay developer access token.
3. Run all cells.

## Data Source
Data was retreived using the eBay Browse API.

## License
This project is licensed under the MIT License.