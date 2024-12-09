# Grocery Price Inflation 

It is no surprise that grocery prices have gone up. [NPR Article](https://www.npr.org/2024/09/09/nx-s1-5103935/grocery-prices-inflation-corporate-greedflation) [NY Times Article](https://www.nytimes.com/2024/08/15/business/economy/kamala-harris-inflation-price-gouging.html). 
The purpose of this project is to figure out if the [largest retail grocery stores](https://www.foodindustry.com/articles/top-10-grocers-in-the-united-states-2019/#gsc.tab=0) are inflating their prices above standard inflationary rates to drive up profits post-pandemic, a term coined as ['greed-flation'](https://cssh.northeastern.edu/what-is-greedflation-and-is-it-driving-higher-prices/).

In this analysis I set out to find if the top retail grocery stores are exploiting consumers by hiking up prices, and taking advantage of the market. The data used are financial statements (income statement, balance sheet, and cash flow) that were extracted from Alpha Vantage's library from companies such as: Kroger, Albertsons, General Mills, Walmart and Costco.

**Tech used:** Python (libraries include Pandas, OS, Matplotlib, and Alpha Vantage)

**Notebook can be found [here](https://github.com/JasonSTLee/Greed-Flation/blob/main/alpha_api.ipynb)**

## Questions to ask

**1.** Is there an increase of revenue and profits for the companies?
![revenue profit](https://github.com/user-attachments/assets/131a82c6-a99f-4d84-849d-cad359fbd53d)

In all cases since the pandemic, all grocery stores have increased revenue and profit year over year besides Kroger in 2023. However this one year with one company is the exception rather than the rule. 

---

**2.** What are post and pre-pandemic growth like? Are companies taking advantage of people more post-pandemic?
![output2](https://github.com/user-attachments/assets/db1e70a7-19e9-48b6-8bfd-52d3265b8ab6)

While the average YoY total revenue has grown, profits have not been keeping up. This could mean that cost of operations has gone up while revenue has gone up as well. However the costs may be increasing faster than revenue. Profit growth has declined post-pandemic significantly, suggesting that the pandemic has shifted margins in the retail grocery industry.

---

**3a.** Are companies more profitable now than before the pandemic?
![output3](https://github.com/user-attachments/assets/ce83b5e0-c3e6-41e0-b166-94ae63699983)

ROCE (Return on Capital Emplyed) and ROA (Return on Assets) are 2 financial metrics that measure a company's profitability. ROCE focuses on how well a company uses itc capital to generate profits. ROA focuses on how efficiently a company uses all of its assets to generate profit. Both ROCE and ROA have been declining since 2016 and have not returned to those highs ever since. While there have been an increase during and a few years after the pandemic, returns fell in 2024. This _could_ indicate that companies are more efficient in generating profits post-pandemic, however the increase isn't as large to indicate greed-flation.

**3b.** 
![5](https://github.com/user-attachments/assets/fde6166d-09f6-451e-a235-5513160a90a0)

Gross margin is the percentage of a company's revenue that's retained after direct expenses such as labor and materials have been subracted. Kroger and Albertsons have shown a hike in gross margin after the pandemic while Walmart saw a slight increase and Costco fell from the year prior. However most of the companies after 2021 dropped in gross profit margin. Companies may increase price of goods if gross margins are down as a revenue-increasing measure. This could explain why consumers are feeling 'greed-flation' but this isn't due to companies wanting to maximize profits, but rather returning to a healthy state of profits. 

---

**3c.** 
![operation](https://github.com/user-attachments/assets/cfbdfcda-aebf-46fc-bd5e-1b6b62ab800c)

Operating margins represents how efficiently a company is able to generate profits through its core operations. There has been continual growth even before the pandemic, with a spike in 2022 followed by 2 years of decline. This indicates that the core operation (selling groceries to consumers) have been dropping in efficiency 2 years in a row. 

---

**3d.** 
![asdf](https://github.com/user-attachments/assets/4372e3bd-4e2c-4893-abac-4e1a57d775ad)

Nearly identical to the operating margins graph, free cash flow (measures percentage of reveneue that is converted to cash) spiked after pandemic and came crashing down years later. 

---

## Conclusions

Based on my analysis of the financial statements of major retail grocery companies, there is no strong evidence to indicate that major retail grocery companies are exploiting consumers by hiking up prices for their own selfish gain, but rather keeping their operations and business healthy. While there was a **spike in operation margins and free cash flow, the increase started in 2019 and not 2020** when the pandemic occurred, suggesting that these changes were not solely driven by the pandemic. Additionally, gross margin over time hasn't seen a notable increase, in fact **all companies have a lower gross margin in 2024 than compared to 2010** (2018 in Albertsons case due to lack of data). Despite revenue and profits increasing year over year, after digging deeper we are able to see that operations are not as efficient, and available cash is lower than their previous, recent highs. This indicates that the improvements in financial performance is due to reasons outside of inflating their price, or rather there is a price increase due to operational inefficiencies. 

The [Federal Reserve Bank of New York City](https://libertystreeteconomics.newyorkfed.org/2024/07/what-was-up-with-grocery-prices/) makes a claim that the higher grocery prices post-pandemic is not caused by inflation but higher wages:
> [there is an] increase in these workers’ wages since 2019 has been roughly 15 percentage points

and

> Grocery worker wages would seem then to be a key factor in why the food index has gone up more than the core price index.


### Limitations of Dataset
1. Albertsons data only shows 2018 onward while the other companies had financial statements from 2010
2. While financial statements are important, they only show a snapshot in time for a particular company, not broader economic information
