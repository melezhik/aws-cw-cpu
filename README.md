# SYNOPSIS

Sparrow plugin to show `CPUUtilization` for ec2 instance.

# INSTALL

    $ sparrow plg install aws-cw-cpu

# USAGE

To get CPU load for the last 2 weeks with daily granularity:

    $ sparrow plg run  aws-cw-cpu --param id=$instance-id --param range='2 weeks'


The same instance, for the last 10 days:

    $ sparrow plg run  aws-cw-cpu --param id=$instance-id --param range='10 days'

# Parameters

## range

Should be in format of: `$N weeks|days|hours`


# Output example:

```
CPU Load Stat
InstanceID: i-09****b6006847*****
range: 7 days (2017-09-20 / 2017-09-27)
┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃2017-09-20 00.67%:▅                                                                                                            ┃
┃2017-09-21 00.83%:▅▅                                                                                                           ┃
┃2017-09-22 00.68%:▅                                                                                                            ┃
┃2017-09-23 00.66%:▅                                                                                                            ┃
┃2017-09-24 00.83%:▅▅                                                                                                           ┃
┃2017-09-25 00.83%:▅▅                                                                                                           ┃
┃2017-09-26 88.62%:▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅▅┃
┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛

```

# Author

Alexey Melezhik

# Prerequisites

Aws cli should be installed

