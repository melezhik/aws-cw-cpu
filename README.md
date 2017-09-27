# SYNOPSIS

Sparrow plugin to show `CPUUtilization` for ec2 instance.

# INSTALL

    $ sparrow plg install aws-cw-cpu

# USAGE

To get CPU load for the last 2 weeks with daily granularity:

    $ sparrow plg run  aws-cw-cpu --param id=$instance-id --param range='2 weeks'

# Author

Alexey Melezhik

# Prerequisites

Aws cli should be installed

