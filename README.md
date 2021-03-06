# Build latest [guetzli](https://github.com/google/guetzli) for CentOS / RedHat 6, 7, 8

|CI|Purpose|Status|
|---|---|---|
| CircleCI | Builds `guetzli` for [GetPageSpeed repository](https://www.getpagespeed.com/redhat) (fast CDN repo) | [![CircleCI](https://circleci.com/gh/GetPageSpeed/guetzli-rpm.svg?style=svg)](https://circleci.com/gh/GetPageSpeed/guetzli-rpm) |

If you use CentOS / RHEL 6, 7 or 8, it is highly recommended to install `guetzli` from GetPageSpeed repository:

    sudo yum install https://extras.getpagespeed.com/release-el$(rpm -E %{rhel})-latest.rpm
    sudo yum install guetzli

Install helper program for comparing Guetzli encoded images vs original:

    sudo yum installl guetzli-compare