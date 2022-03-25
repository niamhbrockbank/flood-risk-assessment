# Flood Risk Assessment
This report quantifies the flood risk to the proposed residential development to the east of Bath. The findings are based on AMAX data recorded by the gauging station on the By Brook, north east of Bath, location shown in Figure 1 Catchment Area.

<img width="549" alt="image" src="https://user-images.githubusercontent.com/67958003/160144554-bb8860da-f681-417c-8147-3c8e6255fd77.png">

## 1 AMAX Data Summary
The available AMAX data, recorded at the station on By Brook, covers years 1981 to 2015 inclusive. The full dataset is shown in Table 1-1.
* Highest peak flow rate- 19.63 m3/s (recorded 1986)
* Lowest peak flow rate- 5.52 m3/s (recorded 1999)
* Mean peak flow rate- 10.64 m3/s

<img width="404" alt="image" src="https://user-images.githubusercontent.com/67958003/160145636-52a8e287-334e-4516-918a-9933a7c4db47.png">

<img width="625" alt="image" src="https://user-images.githubusercontent.com/67958003/160145907-01641f7a-442e-4e22-9c50-7a1b90cc3f04.png">

### 1.1 Data Limitations
No data is available from the other local watercourses, it is therefore assumed that the development will not be affected by their flood zones.

The reliability of the dataset’s application to the proposed development area is directly proportional to its proximity to the By Brook gauging station. The risk of flooding reduces the further from the watercourse, therefore this inaccuracy is deemed conservative.

The data is limited by the length of the available record (35 years), and the maximum and minimum peak flow rates which were recorded. Extrapolation is required to estimate beyond the record’s range.

## 2 Flood Distribution Investigation
The most accurate way of extrapolating the data to beyond its range is to assign a statistical frequency distribution to it. This assumes the statistical behaviour of the floods will remain the same for extreme events. In this risk assessment, the Gumbel distribution will be used.

### 2.1 The Gumbel Distribution
The Gumbel distribution can be used to calculated a 'T'-year design flood, x_T, using forumla (1).

<img width="635" alt="image" src="https://user-images.githubusercontent.com/67958003/160146294-bfb2dd3f-d6bb-4b1f-ac5a-ac056f6beea6.png">

The Gumbel distribution is commonly used for flood risk assessments, in Section 2.2 the “Goodness of Fit” of this distribution will be verified for this data set.

#### 2.1.1 Gringorten Plotting Position Modification
The Gringorten plotting position formula modifies the data to reflect its limitations (duration of recording and extreme values) without making any distributional assumptions.

The AMAX data given in Table 1-1 is used with the Gringorten plotting position formula (2) to determine the modified return period for each of the n events, see Table 7-1 for all data, and hence the plotting positions on Figure 3 Empirical Frequency Distribution obtained using Gringorten.

<img width="627" alt="image" src="https://user-images.githubusercontent.com/67958003/160147005-5938be23-8c5d-4a0c-ab55-dc3e35655c03.png">

<img width="556" alt="image" src="https://user-images.githubusercontent.com/67958003/160147062-2045fc77-8330-4f02-9c78-64c57c1be2c6.png">

#### 2.1.2 Gumbel Reduced Variate
The return periods, derived from this formula have then been used to calculate the Gumbel Reduced Variate, y_T, using equation (3), see Table 7-1 for all data.

<img width="627" alt="image" src="https://user-images.githubusercontent.com/67958003/160147309-a8a3f8ba-9e61-4fe4-a476-883be576fa0b.png">

This is then used in Equation (1), alongside the two model parameters, 𝛼 and mu, which are estimated using the following:

<img width="633" alt="image" src="https://user-images.githubusercontent.com/67958003/160147760-62b9ad53-741d-4eae-a3f4-2d7e7f298c46.png">

The results of these calculations are used to plot the Gumbel distribution “line” against the modified data as shown in Figure 4.

<img width="620" alt="image" src="https://user-images.githubusercontent.com/67958003/160147952-9ba54e1e-af34-4586-baf8-9482f14f30cb.png">

### 2.2 Goodness-Of-Fit
A visual assessment of Figure 4 suggests the Gumbel distribution describes the statistical frequency of this data well. This visual assessment can be confirmed by conducting a Chi^2 statistical test.

#### 2.2.1 Chi^2 Statistical Test
The Chi^2 statistical test is used to assess the “goodness-of-fit” of the Gumbel distribution to the gauging station data. The Chi^2 statistical test will verify or falsify the null hypothesis.

* **Null Hypothesis, H0:** The Gumbel distribution is a valid choice of distribution. 
* **Alternative Hypothesis, H:** The Gumbel distribution is not a valid choice of distribution.

The data is split into equal probability bins, the number of bins, k, is determined by 𝒌 = n/5, where n is the number of available AMAX observations. The upper bin levels, x_i, (the largest flow in each bin are shown in Table 2-1.

<img width="580" alt="image" src="https://user-images.githubusercontent.com/67958003/160148617-c7c7bd04-1f88-43b0-be2e-86de2ba65b91.png">

The test statistic Chi^2 is calculated from this data using the following formula:

<img width="646" alt="image" src="https://user-images.githubusercontent.com/67958003/160148714-16426448-964f-454b-8de8-87061a76a66e.png">

The Chi^2 value for this dataset is, therefore:

<img width="613" alt="image" src="https://user-images.githubusercontent.com/67958003/160148816-6ab15bf6-bef1-47a2-a2f3-aa3d272729ac.png">

This test has 4 degrees of freedom, as Gumbel distributions have 2 estimated parameters. The significance level is given at 1% to ensure the most conservative estimate, due to the nature of the planned development. This gives the critical value of Chi^2 for a test of this nature.

<img width="599" alt="image" src="https://user-images.githubusercontent.com/67958003/160148884-84e20e78-a7c9-4fd3-acfc-1d4b6d2769a1.png">

Therefore, the Gumbel distribution is a valid choice of distribution.

## 3 Design Floods
The design flow rates have been calculated using the Gumbel distribution and can be seen below in Table 3-1 Design Floods and Confidence Intervals. Using a confidence interval of 95%, the following upper and lower bound design flow rates have also been found.

The standard deviation is found using:
<img width="628" alt="image" src="https://user-images.githubusercontent.com/67958003/160149131-e766d99b-8fb9-42c6-aac9-2b5951f21007.png">

<img width="645" alt="image" src="https://user-images.githubusercontent.com/67958003/160149221-b5caebc8-67d8-4c36-a9e3-c04065e4e650.png">
<img width="640" alt="image" src="https://user-images.githubusercontent.com/67958003/160149271-ae94e69c-158f-4694-a824-b6fd2ba398ac.png">

<img width="664" alt="image" src="https://user-images.githubusercontent.com/67958003/160149305-c1cfd0b3-5c52-44c8-8bac-2f9e649d5492.png">

The x_100 and x_200 design flows are outside the range of recorded data, and therefore will have the greatest uncertainty.

## 4 Climate Change Assessment
Climate change is expected to increase the severity of flooding events, this must be taken into account for any long-term design. This location, east of Bath, is considered to be in ‘Flood Zone 2’ (See Table 7-2) and dwelling houses are considered ‘More Vulnerable Infrastructure’ (See Table 7-3). Therefore, the government recommendation is to use the ‘Central Higher’ and ‘Upper End’ allowance categories to anticipate the potential percentage change of peak river flow.

<img width="616" alt="image" src="https://user-images.githubusercontent.com/67958003/160149684-08b76006-31da-4060-8c4d-079cd11aef52.png">

Current climate change predictions do not extend further than 2115, so it would be unreasonable to give an estimate for the 200-year return period beyond that it will be larger than for the 100- year return period.
