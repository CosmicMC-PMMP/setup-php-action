<p align="center">
  <a href="https://github.com/CosmicMC-PMMP/setup-php-action/actions"><img alt="setup-php-action status" src="https://github.com/CosmicMC-PMMP/setup-php-action/workflows/build-test/badge.svg"></a>
</p>

# setup-php-action

This action installs PHP and Composer for [CosmicMC-PMMP](https://github.com/CosmicMC-PMMP/PocketMine-MP) from [CosmicMC-PMMP/PHP-Binaries releases](https://github.com/CosmicMC-PMMP/PHP-Binaries/releases).

This is used internally for CosmicMC-PMMP's own CIs, and can also be used by plugins using GitHub Actions.

Currently only supported on Linux, but MacOS and Windows support is planned for the future.

## Inputs
| Name | Required | Possible values | Description |
|:-----|:--------:|:----------------|:------------|
| `php-version` | YES | Any version available in [`CosmicMC-PMMP/PHP-Binaries`](https://github.com/CosmicMC-PMMP/PHP-Binaries) (currently `8.1` through `8.5`) | PHP version, must be a full `major.minor.patch` |
| `install-path` | YES | Folder path | Path to install the binary into (e.g. `./bin`) |
| `pm-version-major` | NO | `5` | Major version of [CosmicMC-PMMP](https://github.com/CosmicMC-PMMP/PocketMine-MP) to build extensions for |
