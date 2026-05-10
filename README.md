# Astronomical Infrared Excess Analysis

This project analyzes astronomical infrared flux data from the SEIP catalog to identify possible infrared-excess candidates. Infrared excess can suggest objects with additional dust emission, making it useful for exploring stars, galaxies, or other sources with unusual infrared behavior.

## Project Overview

The analysis uses infrared flux measurements at multiple wavelengths, including 3.6 micron, 4.5 micron, 8.0 micron, and 24 micron bands. The main goal is to compare the 24 micron flux against shorter infrared bands and identify objects with unusually high long-wavelength emission.

## Methods Used

- Cleaned astronomical flux data by removing missing, infinite, and non-positive values
- Created ratio-based features comparing 24 micron flux to shorter infrared wavelengths
- Applied log transformations to handle large flux ranges
- Defined an infrared-excess score using log10(m1 / i1)
- Flagged the top 5% of objects as infrared-excess candidates
- Used K-Means clustering to explore structure in the engineered feature space
- Applied PCA to visualize high-dimensional infrared features in two dimensions

## Tools and Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

## Key Skills Demonstrated

- Data cleaning
- Feature engineering
- Unsupervised machine learning
- Clustering
- Principal Component Analysis
- Scientific data analysis
- Astronomical data interpretation

## Results

The project identifies candidate objects with unusually high 24 micron emission relative to shorter infrared wavelengths. These candidates are visualized using histograms, ratio-based scatter plots, K-Means clusters, and PCA projections.

## Future Improvements

- Compare candidates against known astronomical object labels
- Add additional wavelength bands or color-color diagrams
- Test different candidate thresholds besides the top 5%
- Export candidate objects into a separate CSV file
- Improve visualizations for presentation and publication
