# Binder environments for ArviZ libraries
This repo is used to store and publish binder environments
to be used by ArviZ libraries to better integrate
their documentation with binder and thebe.

Ideally, for faster loading and trying to optimize caching
on the binder side, libraries will have their own
repo in a specific branch, with a minimal environment
and all dependencies listed out explicity
from a `requirements.in` using [`pip-compile`](https://github.com/jazzband/pip-tools#example-usage-for-pip-compile)
however, especially at first, "raw" `requirements.txt` can also be used.

The `main` branch will have a base environment for quick testing
that installs bare bones ArviZ (python only for now) and ArviZ libraries
without `pip-compile` use for fast iteration and prototyping.
