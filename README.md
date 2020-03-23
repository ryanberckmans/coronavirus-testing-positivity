
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

## Example output (actual data as of 2020/3/23)

```
For 1 days ending 20200323
  total case growth    US: 32.2%     SK: 0.7%
  total test growth    US: 28.8%     SK: 1.9%
  positivity rate      US: 19%       SK: 0.9%

For 2 days ending 20200323
  total case growth    US: 81.7%     SK: 1.8%
  total test growth    US: 61%       SK: 3.2%
  positivity rate      US: 18.9%     SK: 1.3%

For 3 days ending 20200323
  total case growth    US: 147.5%    SK: 3.6%
  total test growth    US: 112.3%    SK: 6.7%
  positivity rate      US: 17.4%     SK: 1.3%

FAQ
  Q: Which data?
  A: Data for just USA from https://covidtracking.com

  Q: What's "total case growth"?
  A: Percent growth in total cumulative people with the virus.

  Q: What's "total test growth"?
  A: Percent growth in total cumulative tests done to see if people have the virus.

  Q: What's "positivity rate"?
  A: Percent of newly tested people that test positive, ie. do have the virus.

  Q: What's up with "percent of newly tested people that have the virus"?
  A: In South Korea this number is about 1%. Ie. in South Korea 99% of people
     newly tested for covid don't have the virus. If America can get this
     number lower then that may be evidence that we are starting to control
     the virus.
```
