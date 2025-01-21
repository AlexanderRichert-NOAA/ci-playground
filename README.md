![workflowstatus](https://github.com/AlexanderRichert-NOAA/ci-playground/actions/workflows/build.yaml/badge.svg)

Packages that must be provided by GitHub Actions workflows using these packages:
- Spack (to concretize environment and access/install from build cache)
- Compilers (GCC, Intel Classic, Intel OneAPI; see .github/workflows/test.yaml for available versions; use apt or https://github.com/NOAA-EMC/ci-install-intel-toolkit to install)
- Intel MPI (see .github/workflows/test.yaml for available versions; use apt or https://github.com/NOAA-EMC/ci-install-intel-toolkit to install)

To use the build cache, run the following prior to concretizing and installing a Spack environment:
```console
$ spack mirror add emc-build-cache oci://ghcr.io/AlexanderRichert-NOAA/ci-playground
```
