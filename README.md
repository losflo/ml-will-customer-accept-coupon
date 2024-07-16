# Will a Customer Accept the Coupon?

For the detailed steps I used in this analysis, please refer to [Jupyter Notebook](https://github.com/losflo/ml-will-customer-accept-coupon/blob/main/prompt.ipynb)

### Problem 
With the included data, find out which customer group will accept the coupon the most to increase marketing efforts for these groups of people.

### Findings
My findings for who accepts bar coupons is based on `age` and frequency they go to Bars. `age` displayed the highest approval rates at ages 21, 26, 31 tapering down the you go older. Frequency saw an net accepted response above once a month. The approval rate for frequencies of less than once a month was so bad, I would recommend to stop targeting this group at all.

## Conclustion
When combining these factors I saw an increase in approval rates. The area I'd target for marketing of what already works would be the group in which: ages are 21-31, and frequency of bar visits is greater than once a month.

### Independent Inventigation
I've choosen my coupon type to be 'Coffee House'. The purpose of my investigation will be to see what group of people use the most coupons to increase marketing for these groups. The 'Next Steps' section will be dedicated to attempting to increase volume in the area that isn't working. Essentially taking the filters from the primary investigation and performing the same steps to find a correlation in the 'less' approving group.

### Coffee House Conclusion
I found `occupation`, `age`, and frequency of visits are the three highest indicators *individually* for whether a coupon will be Accepted or not. I then attempted to combine those filtered sets to see if it correlated to a higher acceptance rate. Combining these indicators resulted in a 90% acceptance rate. This is a rather high acceptance rate which may indicate a rather small set of data that fits the defined filter. I found the dataset for this Acceptance Rate to only be 50 in count. Before any marketing budget would be spent on this, more data would need to be collected to ensure the Acceptance Rate holds true in a larger data set.

Assuming this would hold true in a larger dataset, my recommendation would be as follows. Target the group in which occupation is in `Healthcare Practitioners & Technical` and `Building  Grounds Cleaning & Maintenance`, go to a Coffee House more than 1 time a month and are greater than the age of 25.


## Next Steps
As mentioned above, this section of the investigation will take a dive into some of the 'less' Approving groups. The purpose of this is to uncover a correlation to acceptance in the subset of data to increase the coupon usage.

## Next Steps Hypothesis
To answer this question
1) let's omit the datapoints we used to find what is already working
2) Rerun the acceptance rate calculations on each field
3) analyze the calculations to see which fields hold the most weight in the less effective set of data.
4) choose the fields along with the filter to specifically target those indicators to increase coupon use.

### Next Steps (Conclusion)

I found once again that `occupation` is the greatest indicator of whether the coupon will be used or not. However, in this case the occupation with the highest acceptance rate is `Office & Administrative Support` with a lower volume. With this in mind I would also use the `Student` occupation as it has a larger volume to target a larger group of people. My recommendation to increase coupon use would be to target individuals with occupation `Office & Administrative Support` or `Student` and are under the age of 25.

The same problem arises in this sub-investigation. Volume. Out of 12K data points, would you make a decision based on 600 datapoints that would require investing money into? My thought would be no. I believe data analysis is a dance between finding a correlation in a big enough subset of data to be confident enough to make decisions off of. How large would this subset of data need to be? Personal or Company preference would be my guess.

For the detailed steps I used in this analysis, please refer to [Jupyter Notebook](https://github.com/losflo/ml-will-customer-accept-coupon/blob/main/prompt.ipynb)