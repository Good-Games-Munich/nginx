[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

<!-- PROJECT HEADER -->
<br />
<p align="center">
  <!-- https://github.com/stefanjudis/github-light-dark-image-example -->
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.github.com/Good-Games-Munich/assets/main/logos/GGM_logo_white.png">
    <img alt="Logo" src="https://raw.github.com/Good-Games-Munich/assets/main/logos/GGM_logo_black.png" height="150">
  </picture>

  <h3 align="center">🛣️ Nginx</h3>

  <p align="center">
    ·
    <a href="https://github.com/Good-Games-Munich/nginx/issues">Report Bug</a>
    ·
    <a href="https://github.com/Good-Games-Munich/nginx/issues">Request Feature</a>
    ·
  </p>
</p>

<!-- ABOUT THE PROJECT -->

## About The Project

Setup for nginx to automatically generates nginx configurations and renew Let´s Encrypt certificates.
Routes traffic to the corresponding containers.

## Setup

### Production

Follow [Creating a release](https://github.com/Good-Games-Munich/.github/wiki/workflows#creating-a-release).

### Development

1. Follow [local setup](https://github.com/Good-Games-Munich/.github/wiki/workflows#local-setup).
2. Follow the [Customization](#customization) section and set all variables with `Required in dev` `true`.
3. Add a `127.0.0.1 localtest.me` entry in your host file. See [How to edit host files](https://www.hostinger.com/tutorials/how-to-edit-hosts-file)
4. Navigate to `http://localtest.me`

### Customization

Create a environment file `touch .env`. Override variables in the `{variable name}={variable value}` format. All required variables need to be overridden for the respected environment.

| Variable        | Description                                   | Required in dev | Required in prod | Default value |
| --------------- | --------------------------------------------- | --------------- | ---------------- | ------------- |
| `DEFAULT_EMAIL` | Defines your default email for Let's Encrypt. | `true`          | `true`           | none          |

<!-- CONTRIBUTING -->

## Contributing

Follow [contributing](https://github.com/Good-Games-Munich/.github/wiki/workflows#contributing).

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/Good-Games-Munich/nginx.svg?style=flat-square
[contributors-url]: https://github.com/Good-Games-Munich/nginx/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Good-Games-Munich/nginx.svg?style=flat-square
[forks-url]: https://github.com/Good-Games-Munich/nginx/network/members
[stars-shield]: https://img.shields.io/github/stars/Good-Games-Munich/nginx.svg?style=flat-square
[stars-url]: https://github.com/Good-Games-Munich/nginx/stargazers
[issues-shield]: https://img.shields.io/github/issues/Good-Games-Munich/nginx.svg?style=flat-square
[issues-url]: https://github.com/Good-Games-Munich/nginx/issues
