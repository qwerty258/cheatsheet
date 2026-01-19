zypper
======

|Command                            |Description                                    |Example                                            |
|-----------------------------------|-----------------------------------------------|---------------------------------------------------|
|`zypper refresh`                   |Refreshes repository data                      |`zypper refresh`                                   |
|`zypper update`                    |Updates all installed packages                 |`zypper update`                                    |
|`zypper install PACKAGE_NAME`      |Installs a specified package                   |`zypper install vim`                               |
|`zypper remove PACKAGE_NAME`       |Removes a specified package                    |`zypper remove vim`                                |
|`zypper search PACKAGE_NAME`       |Searches for a package in the repositories     |`zypper search firefox`                            |
|`zypper info PACKAGE_NAME`         |Displays detailed package information          |`zypper info firefox`                              |
|`zypper list-updates`              |Lists all packages with available updates      |`zypper list-updates`                              |
|`zypper dist-upgrade`              |Performs a distribution upgrade                |`zypper dist-upgrade`                              |
|`zypper clean`                     |Cleans up cached repository data               |`zypper clean`                                     |
|`zypper addrepo URL ALIAS`         |Adds a new software repository                 |`zypper addrepo http://repo.url/ custom-repo`      |
|`zypper removerepo ALIAS`          |Removes a software repository                  |`zypper removerepo custom-repo`                    |
|`zypper repos` or `zypper lr`      |Lists all currently configured repositories    |`zypper repos`                                     |
|`zypper lr -u`                     |include repo URI on the table                  |                                                   |
|`zypper lr -P`                     |include repo priority and sort by it           |                                                   |
