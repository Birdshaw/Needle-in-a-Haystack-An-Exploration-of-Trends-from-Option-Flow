Needle in a Haystack: An Exploration of Trends from Option Flow
===
An exploratory data analysis of stock option flow to find possible trends regarding future price movement and manipulation.
---

**Project Summary:**
---

In the past as it is today, institutional investors are able to hide their trades from the general public. However it was discovered that by looking at the volume of a stock one could ascertain where those investors were putting their money and in turn get an idea of potential future market trends. 

However, with the improved technology that retail investors (us normal people) have to work with, the ways in which they must hide their trades have increased. As such, the ability for traditional stock volume to be an indicator for institutional investing movement and insight has decreased. 

In its place their exists another kind of volome to explore called option volume or option flow. This data is something that is not readily available or utilized but can hold the same power as traditional stock volume. The goal of this project is to explore what trends can be seen in stock option flow and discern any correlations their may be to future stock movement. 

---
**Project Overview:**
---

*Dataset:*

The dataset for stock option flow used came from the website https://www.discountoptiondata.com. I used the stock option flow dataset for 2018. It consists of an aggregate of all stocks daily option volume data related to its strike price and expiration date. 

The traditional stock time and price datasets were pulled from https://www.barchart.com. Which allows you to pick stocks at will and download a stocks minute, hourly, or daily data for any specified time period. For this project I used the dialy 2018 time period to coincide with the aforementioned option flow data.

| File/Folder Name | Number of Entries | Attributes | Notes |
| --------------- | ---------------| ------------------------------------------------------------| ----------|
| 2018/ | 132,046,568 | optionkey, Symbol, ExpirationDate, AskPrice, AskSize, BidPrice, BidSize, LastPrice, PutCall, StrikePrice, Volume, openinterest, underlyingPrice, DataDate | Data split into .csv's by month of the year
| <stock>.csv | 642 | Date Time, Open, High, Low, Close, Change, Volume | Used multiple different stock datasets but all have identical number of entries and attributes. |

**EDA Plots**
---

*Visual example data to be analyzed for correlation by exploring relationship between a stock options expiration date, strike price, and volume. Important points are the peaks on this graph and where they correspond to date and price.*
 
 ![Option flow plot for a day](/img/tsla0116flow.png)
 
*Correlate these peaks in stock option flow to either its corresponding day or expiration date as seen below.*

![](/img/exp_tsla_with_price.png)

*From here we can visualize the number of potential successful trades per month based on top two highest volume peaks. Below are the successes (in red) and failures (in green) of potential trades for Telsa and Netflix.*

![](/img/tsla_Jan_peak_option.png)

![](/img/nflx_Jan_peak_option.png)

*To expand the analysis a view of the year as a whole is in order by both daily and expiration date sell for various stocks. These display the total number of successful trades and the percentage of successful trades in each month.*

![](/img/NFLX_Summary_2018.png)

![](/img/AMD_Summary_2018.png)

![](/img/FB_Summary_2018.png)

![](/img/BA_Summary_2018.png)

![](/img/BABA_Summary_2018.png)

![](/img/DIS_Summary_2018.png)

![](/img/GOOGL_Summary_2018.png)

![](/img/HD_Summary_2018.png)

![](/img/JPM_Summary_2018.png)

![](/img/SHOP_Summary_2018.png)

![](/img/WYNN_Summary_2018.png)




