# Exploratory Data Analysis Report

## Variable Descriptions
- **Timestamp** → Date and time of the measurement
- **GHI (Global Horizontal Irradiance), DNI (Direct Normal Irradiance), DHI (Diffuse Horizontal Irradiance)** → Solar radiation values
- **ModA, ModB** → Possibly sensor module data (need clarification)
- **Tamb** (Ambient Temperature), TModA, TModB → Temperature readings
- **RH** (Relative Humidity) → Air moisture level
- **WS** (Wind Speed), WSgust (Wind Gust), WSstdev (Wind Speed Standard Deviation) → Wind data
- **WD** (Wind Direction), WDstdev (Wind Direction Standard Deviation) → Wind movement
- **BP** (Barometric Pressure) → Air pressure
- **Cleaning** → Might indicate sensor cleaning status
- **Precipitation** → Rainfall levels

## Data Quality Check
- **Null Values**: No null values were found in any of the DataFrames.
- **Column Dropped**: The 'Comments' column was dropped from all three DataFrames.

## Summary Statistics
The analysis revealed that Benin-Malanville has the highest average Global Horizontal Irradiance (GHI) of **241.96 watts per square meter**, making it the best location for solar installation among the three sites.

## Average Wind Speeds (m/s)
- **Benin-Malanville**: 2.12
- **Sierra Leone-Bumbuna**: 1.15
- **Togo-Dapaong**: 2.37

## Visualizations

### Solar Radiation Trends
The solar radiation trends for each location show varying levels of GHI over time, with Benin displaying the highest peaks in solar irradiance. Both Sierra Leone and Togo show consistent trends, but with lower maximum values compared to Benin.


### Frequency Distribution of DNI
The histograms illustrate the frequency distribution of Direct Normal Irradiance (DNI) across the three locations, indicating that most readings are clustered near zero. Benin exhibits a broader range of values compared to Sierra Leone and Togo, suggesting more variability in solar conditions.


### Correlation Between Variables
The correlation matrix for Benin shows strong positive correlations between GHI, DNI, and DHI, indicating that as one increases, the others tend to increase as well. Additionally, temperature (Tamb) exhibits a moderate correlation with humidity (RH), suggesting that higher humidity may be associated with higher temperatures.


### Impact of Cleaning on Sensor Readings
The bar charts show the average sensor readings for ModA and ModB before and after the cleaning process, highlighting improvements in the data quality across all three locations. Benin demonstrates the highest average readings, indicating more reliable sensor performance.


## Conclusion
Based on the analysis, Benin-Malanville is identified as the most suitable location for solar installation, thanks to its favorable GHI and consistent solar radiation trends. The data cleaning process has enhanced the reliability of the sensor readings, providing a solid foundation for further analysis and implementation.