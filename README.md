
# A daily coronavirus report on the command line

It's a nodejs script with zero dependencies. You don't need to install node_modules.

Quick start

```bash
cd /tmp && git clone --quiet https://github.com/ryanberckmans/coronavirus.git && cd coronavirus && ./report
```

## Example output (actual data as of 2020/3/21)

```
For 1 days ending 20200321
  percent growth in total cumulative people with the virus: 36.2%
  percent growth in total cumulative tests done to see if people have the virus: 31.8%
  percent of people newly tested that have the virus: 14%

For 2 days ending 20200321
  percent growth in total cumulative people with the virus: 97.9%
  percent growth in total cumulative tests done to see if people have the virus: 75.8%
  percent of people newly tested that have the virus: 14.7%

For 3 days ending 20200321
  percent growth in total cumulative people with the virus: 200.1%
  percent growth in total cumulative tests done to see if people have the virus: 138.7%
  percent of people newly tested that have the virus: 14.7%

FAQ
  Q: Which data?
  A: Data for just USA from https://covidtracking.com

  Q: What's up with "percent of people newly tested that have the virus"?
  A: In South Korea this number is about 1%. Ie. in South Korea 99% of people
     newly tested for covid don't have the virus. If America can get this
     number lower then that may be evidence that we are starting to control
     the virus.
```
