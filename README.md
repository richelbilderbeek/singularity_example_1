# singularity_example_1

Branch   |[![GitHub Actions logo](man/figures/GitHubActions.png)](https://github.com/richelbilderbeek/singularity_example_1/actions)          
---------|------------------------------------------------------------------------------------------------------------------------------------
`master` |![build_singularity](https://github.com/richelbilderbeek/singularity_example_1/workflows/build_singularity/badge.svg?branch=master) 
`develop`|![build_singularity](https://github.com/richelbilderbeek/singularity_example_1/workflows/build_singularity/badge.svg?branch=develop)

Singularity example 1: Hello World.

 * Ubuntu distro: 18.04 (Bionic) 
 * Go v1.12
 * Singularity v3.2.1

## Result

From [a Travis CI build log](https://travis-ci.org/richelbilderbeek/singularity_example_1/jobs/563880368#L2872).

The Singularity container has Trusty:

```
$ singularity exec hello_world.simg cat /etc/os-releas*
NAME="Ubuntu"
VERSION="14.04, Trusty Tahr"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 14.04 LTS"
VERSION_ID="14.04"
HOME_URL="http://www.ubuntu.com/"
SUPPORT_URL="http://help.ubuntu.com/"
BUG_REPORT_URL="http://bugs.launchpad.net/ubuntu/"
```

Travis CI has Xenial:

```
$ cat /etc/os-releas*
NAME="Ubuntu"
VERSION="16.04.6 LTS (Xenial Xerus)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 16.04.6 LTS"
VERSION_ID="16.04"
HOME_URL="http://www.ubuntu.com/"
SUPPORT_URL="http://help.ubuntu.com/"
BUG_REPORT_URL="http://bugs.launchpad.net/ubuntu/"
VERSION_CODENAME=xenial
UBUNTU_CODENAME=xenial
```
