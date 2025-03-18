# Exploratory Data Analysis Report

## Variable Descriptions
- **Timestamp (yyyy-mm-dd hh:mm)**: Date and time of each observation.
- **GHI (W/m²)**: Global Horizontal Irradiance, the total solar radiation received per square meter on a horizontal surface.
- **DNI (W/m²)**: Direct Normal Irradiance, the amount of solar radiation received per square meter on a surface perpendicular to the rays of the sun.
- **DHI (W/m²)**: Diffuse Horizontal Irradiance, solar radiation received per square meter on a horizontal surface that does not arrive on a direct path from the sun.
- **ModA (W/m²)**: Measurements from a module or sensor (A), similar to irradiance.
- **ModB (W/m²)**: Measurements from a module or sensor (B), similar to irradiance.
- **Tamb (°C)**: Ambient Temperature in degrees Celsius.
- **RH (%)**: Relative Humidity as a percentage of moisture in the air.
- **WS (m/s)**: Wind Speed in meters per second.
- **WSgust (m/s)**: Maximum Wind Gust Speed in meters per second.
- **WSstdev (m/s)**: Standard Deviation of Wind Speed, indicating variability.
- **WD (°N (to east))**: Wind Direction in degrees from north.
- **WDstdev**: Standard Deviation of Wind Direction, showing directional variability.
- **BP (hPa)**: Barometric Pressure in hectopascals.
- **Cleaning (1 or 0)**: Signifying whether cleaning (possibly of the modules or sensors) occurred.
- **Precipitation (mm/min)**: Precipitation rate measured in millimeters per minute.
- **TModA (°C)**: Temperature of Module A in degrees Celsius.
- **TModB (°C)**: Temperature of Module B in degrees Celsius.

## Data Quality Check
- **Null Values**: No null values were found in any of the DataFrames.
- **Column Dropped**: The 'Comments' column was dropped from all three DataFrames.

## Summary Statistics
The analysis revealed that Benin-Malanville has the highest average Global Horizontal Irradiance (GHI) of **241.96 watts per square meter**, making it the best location for solar installation among the three sites.

- **Togo-Dapaong**: GHI = **231.72**, DNI = **151.26**
- **Benin-Malanville**: GHI = **241.96**, DNI = **167.44**
- **Sierra Leone-Bumbuna**: GHI = **204.41**, DNI = **116.52**

CSP may not be the better option for Togo-Dapaong compared to Benin-Malanville.

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
Based on the analysis, Benin-Malanville is identified as the most suitable location for solar installation, thanks to its favorable GHI and consistent solar radiation trends. The data cleaning process has enhanced the reliability of the sensor readings, providing a solid foundation for further analysis and implementation. Although Togo-Dapaong has a higher DNI, its lower GHI makes CSP a less favorable option compared to Benin-Malanville.
