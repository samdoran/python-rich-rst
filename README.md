[![Copr build status](https://copr.fedorainfracloud.org/coprs/samdoran/python-rich-rst/package/python-rich-rst/status_image/last_build.png)](https://copr.fedorainfracloud.org/coprs/samdoran/python-rich-rst/package/python-rich-rst/)

# python-rich-rst

* [COPR repo](https://copr.fedorainfracloud.org/coprs/samdoran/python-rich-rst)
* [Upstream repo](https://github.com/wasi-master/rich-rst)
* [Upstream license](https://github.com/wasi-master/rich-rst/blob/main/LICENSE)

## Setup

Before executing a new build, run the initial setup first:

```bash
# Create a new copr repository
make create-copr-repo

# Will create a specfile based on project settings.
# This is only needed in case the python-rich-rst.spec is missing.
make spec
```

## Building

To build this RPM via copr, the following commands are required:

```bash
# Will pull the sources from python-rich-rst.spec and place in the root directory
make sources

# Will perform two operations:
#   * Generate a new srpm with `fedpkg srpm`
#   * Request a new build on copr
make build
```

## Push to Github (optional)

This step is optional, but it will secure that the specfile and other settings
are persisted somewhere.

```bash
# Create a new repository in your account using `gh` and some pre-defined
# settings.
make create-gh-repo
```
