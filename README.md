
# A comparison between the USA and South Korea for the metric of "coronavirus testing positivity rate"

It's a nodejs script with zero dependencies. You don't need to install node_modules.

## Quick start

```bash
cd /tmp && git clone --quiet https://github.com/ryanberckmans/coronavirus.git && cd coronavirus && ./report
```

## About this report

Right now in America we're in a situation where the virus is growing exponentially into the tens of thousands of cases, and testing is ramping up exponentially to essentially attempt to catch up with the virus.

I'm interested in the metric "testing positivity rate" which is the percent of newly tested people that have the virus. Lower is better. The intuition here is that if the government is testing lots of people and 99% of those tested don't have the virus, that may be evidence that the virus is being controlled or at least tracked effectively.

Scott Gottlieb, former commissioner of the FDA, has [written about](https://twitter.com/ScottGottliebMD/status/1241864843008892934) the importance of the testing positivity rate.

## Example output (actual data as of 2020/3/24)

```
FAQ
  Q: Which data?
  A: Data for just USA from https://covidtracking.com

  Q: For X days?
  A: Data for each period is cumulative for that period, not per day. For
     example if the USA has 887 tests per million people over the past 7 days,
     that means all those tests were done over the entire weeklong period,
     that's not 887 per day, it's 887 for the entire week.

  Q: What's "total case growth"?
  A: Percent growth in total cumulative people with the virus.

  Q: What's "total test growth"?
  A: Percent growth in total cumulative tests done to see if people have the virus.

  Q: What's "tests per million"?
  A: The number of tests conducted this period per million people in that country.

  Q: What's "positivity rate"?
  A: Percent of newly tested people that test positive, ie. do have the virus.

  Q: What's up with "percent of newly tested people that have the virus"?
  A: In South Korea this number is about 1%. Ie. in South Korea 99% of people
     newly tested for covid don't have the virus. If America can get this
     number lower then that may be evidence that we are starting to control
     the virus.

For 1 days ending 20200324 
  total case growth    US: 22.4%     SK: 0.8%  
  total test growth    US: 21.7%     SK: 3.1%  
  positivity rate      US: 14.7%     SK: 0.9%  
  tests per million    US: 196       SK: 170   

For 3 days ending 20200324 
  total case growth    US: 122.4%    SK: 2.7%  
  total test growth    US: 96%       SK: 6.4%  
  positivity rate      US: 17.3%     SK: 1.1%  
  tests per million    US: 502       SK: 415   

For 7 days ending 20200324 
  total case growth    US: 801.6%    SK: 8.6%  
  total test growth    US: 551.2%    SK: 21.6% 
  positivity rate      US: 15.8%     SK: 1.1%  
  tests per million    US: 887       SK: 1238
```
