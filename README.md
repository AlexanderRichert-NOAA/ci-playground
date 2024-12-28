![workflowstatus](https://github.com/AlexanderRichert-NOAA/ci-playground/actions/workflows/test.yaml/badge.svg)

Packages that must be provided by GitHub Actions workflows using these packages:
- Spack (to concretize environment and access/install from build cache)
- Compilers (GCC, Intel Classic, Intel OneAPI; see .github/workflows/test.yaml for available versions)
- Intel MPI (see .github/workflows/test.yaml for available versions)
