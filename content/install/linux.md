# Installation on Linux

## System requirements

To install and use the SDK, your development environment must meet these
minimum requirements:

- **Operating systems**: Linux kernel 3.0+ (32-bit or 64-bit)
- **CPU architectures**: x86-64 (amd64), x86 (i386), ARM64 (aarch64), ARM (armhf)
- **Disk space**: 1 MB

## Supported distributions

At present prebuilt binary packages are available for all recent
Ubuntu and Debian releases on the following CPU architectures:

| Distribution     | Alias    | x86-64 |
| :--------------- | :------- | :----- |
| Ubuntu 20.10     | Groovy   | ✔      |
| Ubuntu 20.04 LTS | Focal    | ✔      |
| Ubuntu 19.10     | Eoan     | ✔      |
| Ubuntu 18.04 LTS | Bionic   | ✔      |
| Debian 11        | Bullseye | ✔      |
| Debian 10        | Buster   | ✔      |
| Debian unstable  | Sid      | ✔      |

On other distributions, you can build the SDK from [source code][].

[source code]: https://github.com/conreality/conreality-sdk

## Installation using APT

Once you've completed the [package repository configuration](#configuration)
(see further below), installation is as easy as the familiar:

```bash
$ sudo apt install conreality
```

### Uninstallation

```bash
$ sudo apt purge conreality libconreality20 libconreality-dev libconreality-doc
```

## Configuration

### Configure PGP signing keys

```bash
$ sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 379CE192D401AB61
```

## Configuration on Ubuntu

### Configure on Ubuntu 20.10 (Groovy)

```bash
$ echo 'deb https://dl.bintray.com/conreality/ubuntu groovy main' | sudo tee -a /etc/apt/sources.list
$ sudo apt update
```

### Configure on Ubuntu 20.04 LTS (Focal)

```bash
$ echo 'deb https://dl.bintray.com/conreality/ubuntu focal main' | sudo tee -a /etc/apt/sources.list
$ sudo apt update
```

### Configure on Ubuntu 19.10 (Eoan)

```bash
$ echo 'deb https://dl.bintray.com/conreality/ubuntu eoan main' | sudo tee -a /etc/apt/sources.list
$ sudo apt update
```

### Configure on Ubuntu 18.04 LTS (Bionic)

```bash
$ echo 'deb https://dl.bintray.com/conreality/ubuntu bionic main' | sudo tee -a /etc/apt/sources.list
$ sudo apt update
```

## Configuration on Debian

### Configure on Debian 11 (Bullseye)

```bash
$ echo 'deb https://dl.bintray.com/conreality/debian bullseye main' | sudo tee -a /etc/apt/sources.list
$ sudo apt update
```

### Configure on Debian 10 (Buster)

```bash
$ echo 'deb https://dl.bintray.com/conreality/debian buster main' | sudo tee -a /etc/apt/sources.list
$ sudo apt update
```
