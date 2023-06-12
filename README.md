# linux_social_auth
Builder/Wrapper Repo for linux social auth plugins

## Layout
In the top level repo there is a folder for each of the three components that make up the parts of this project
* linux_social_pam - Custom PAM for OAuth2 authentication using PAM
* linux_social_nss - Custom NSS module that uses either the Keycloak Admin API or SCIM to retrieve user and group information
* linux_social_sudo - Custom sudo module that uses either the Keycloak Admin API or SCIM to perform authorization determination
* linux_social_custom_xrdp - Custom build of xrdp that allows for using OAuth2 as authentication (Not fully supported at the moment since it has issues)

After that there is the top level RPM and DEB specs to build the distro packages.

## Building
In order to build all subprojects and generate a release package you should be on either a Rocky Linux 8/9 machine for the RPM version or a Ubuntu 22 or later for the DEB release. RPM has also been tested with RHEL 8/9.

