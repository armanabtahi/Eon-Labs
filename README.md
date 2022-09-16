# Eon-Labs

This repository is for the TTA for EonLabs, which describes my method in detail.

The data engineering team at Eon Labs conducted some study and discovered that the Google Trends data may be useful to the data science team. I, as a data scientist, require a time series of reliable Google Trends data with hourly intervals from 2018 to the present. I alerted the technical staff of this demand, but they stated that they could not directly retrieve the hourly data. The Deep Dive section explains why they are unable to directly retrieve the hourly data. However, they may obtain the following raw data from Google Trends:

- **hourly_data.csv:** a time series of weekly-consistent Google Trends data starting in 2017 and continuing up to the present, with hourly intervals
- **weekly_data.csv:** a time series of yearly-consistent Google Trends data starting in 2017 and continuing up to the present, with weekly intervals
- **monthly_data.csv:** a time series of consistent Google Trends data starting in 2017 and continuing up to the present, with monthly intervals

They retrieved and concatenated week-range data to obtain a time series of hourly data from 2017 to the present.

They retrieved and concatenated year-range data to obtain the weekly interval time series from 2017 to the present.

By selecting a time range of 2017-present, the engineering team discovered that they could only produce time series of consistent Google Trends data with time intervals of months.

How do you utilise the data files'monthly data.csv,' 'weekly data.csv,' and 'hourly data.csv' provided by the engineering team to generate **time series of consistent Google Trends data from 2018 to the present with time intervals of hours**?
