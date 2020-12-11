About sqlalchemy-jsonfield
==========================

Home: https://github.com/penguinolog/sqlalchemy_jsonfield

Package license: Apache-2.0

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/sqlalchemy-jsonfield-feedstock/blob/master/LICENSE.txt)

Summary: SQLALchemy JSONField implementation for storing dicts at SQL independently
from JSON type support.


Development: https://github.com/penguinolog/sqlalchemy_jsonfield

Documentation: https://github.com/penguinolog/sqlalchemy_jsonfield

SqlAlchemy provides JSON field support for several database types
(PostgreSQL and MySQL for now) and semi-working dict <-> JSON <-> VARCHAR
example, but... In real scenarios we have tests on sqlite, production on
MySQL/MariaDB/Percona/PostgreSQL and some of them (modern Oracle MySQL &
PostgreSQL) support JSON, some of them (SQLite, Percona & MariaDB) requires
data conversion to Text (not VARCHAR).

As addition, we have different levels of Unicode support on database and
connector side, so we may be interested to switch JSON encoding between d
eployments.


Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=8750&branchName=master">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/sqlalchemy-jsonfield-feedstock?branchName=master">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-sqlalchemy--jsonfield-green.svg)](https://anaconda.org/conda-forge/sqlalchemy-jsonfield) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/sqlalchemy-jsonfield.svg)](https://anaconda.org/conda-forge/sqlalchemy-jsonfield) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/sqlalchemy-jsonfield.svg)](https://anaconda.org/conda-forge/sqlalchemy-jsonfield) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/sqlalchemy-jsonfield.svg)](https://anaconda.org/conda-forge/sqlalchemy-jsonfield) |

Installing sqlalchemy-jsonfield
===============================

Installing `sqlalchemy-jsonfield` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
```

Once the `conda-forge` channel has been enabled, `sqlalchemy-jsonfield` can be installed with:

```
conda install sqlalchemy-jsonfield
```

It is possible to list all of the versions of `sqlalchemy-jsonfield` available on your platform with:

```
conda search sqlalchemy-jsonfield --channel conda-forge
```


About conda-forge
=================

[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.com/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](https://anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating sqlalchemy-jsonfield-feedstock
=======================================

If you would like to improve the sqlalchemy-jsonfield recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/sqlalchemy-jsonfield-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@xylar](https://github.com/xylar/)

