**[DEPRECATED] This repository is no longer maintained**
> While this project is fully functional, the content is no longer maintained and therefore is no longer up to date. You are still welcome to explore, learn, and use the code provided here.

# PostgreSQL Box

![No longer maintained](https://img.shields.io/badge/maintenance-OFF-red.svg?&style=flat-square)

Packer templates to build a Vagrant PostgreSQL box.

## Synopsis

This script will create a Vagrant box with PostgreSQL installed and with all
of the required libraries.

## Getting Started

There are a couple of things needed for the templates to work.

### Prerequisites

Packer tools need to be installed on your local computer.

#### Packer

Packer installation instructions can be found [here](https://www.packer.io/docs/installation.html).

#### Vagrant

Vagrant installation instructions can be found [here](https://www.vagrantup.com/docs/installation/).

#### Virtualbox

Virtualbox installation instructions can be found [here](https://www.virtualbox.org/wiki/Downloads).

### Installation

Nothing special to be done. Just download the template that you wish to use.

### Usage

In order to create the box using this packer script you need to provide a
few options.

```
Usage:
  packer build [-var 'option=value'] postgresql.json
```

#### Script Options
- `app_name` - The application name (default value: "postgresql").
- `app_name_ext` - Extra name for the application (default value: "").
- `headless` - Show the console of the machine being built (default value: "true").
- `postgresql_build` - PostgreSQL version build (default value: "1").
- `postgresql_version` - PostgreSQL version (default value: "9.6.1").
- `system_disk_size` - Size of the disk in MB (default value: "12288").
- `system_domain` - Domain name (default value: "marsh").
- `system_hostname` - Host name (default value: "postgresql").
- `system_locale` - Locale for the system (default value: "en_US").
- `system_pwd` - Password for the root and system users (default value: "postgresql").
- `system_timezone` - Time zone for the system (default value: "Europe/Lisbon").
- `system_user` - Username of the system user (default value: "pollywog").

## Services

This box will have the following services running.

| Service    | Port   | Protocol |
|------------|:------:|:--------:|
| SSH        | 22     |    TCP   |
| PostgreSQL | 5432   |    TCP   |

## Contributing

Contributing to this project is no longer possible since the project is no
longer maintained.

## Versioning

This project uses [SemVer](http://semver.org/) for versioning. For the versions
available, see the [tags on this repository](https://github.com/fscm/packer-vagrant-postgresql/tags).

## Authors

* **Frederico Martins** - [fscm](https://github.com/fscm)

See also the list of [contributors](https://github.com/fscm/packer-vagrant-postgresql/contributors)
who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE)
file for details
