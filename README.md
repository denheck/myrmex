<p align="center">
  <h3 align="center">Myrmex</h3>

  <p align="center">Vim configuration generator</p>
</p>


## Table of Contents

* [About the Project](#about-the-project)
* [Getting Started](#getting-started)
  * [Installation](#installation)
* [Usage](#usage)
* [Contributing](#contributing)
* [License](#license)
* [Acknowledgements](#acknowledgements)


## About The Project

This plugin takes a concise convention oriented directory of Vim config files and installs them as Vim8 packages. 

Advantages
* __Independent Source Control:__ Config files are stored in a project folder which can be easily source controlled. No need to get your dotfiles mixed up with your vim packages and .vimrc.
* __Improved Organization:__ One file generates an entire Vim package preventing the need for multiple files and folders.

## Getting Started

To get a local copy up and running follow these simple steps.

### Installation

TODO: explain how to install the CLI tool

## Usage

Once installed the CLI tool can be run like so `myrmex <directory>`, where <directory> is the folder containing the structured configuration files.

The files should be structured like so: `<directory>/<package_name>.vim`

Package files may contain commented out YAML blocks used to delineate sections of Vimscript code in the file. These blocks contain rules for how the code beneath it until the subsequent block or EOF should be loaded. 

An example might be a block describing the code found in the section should be autoloaded only when used:

```
" ---
" autoload: mycommand
" ---
function mycommand#FnRun()
  echo "Run some code"
endfunction
```

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin AmazingFeature`)
5. Open a Pull Request


## License

Distributed under the MIT License. See `LICENSE` for more information.


## Acknowledgements

Thanks to the following exemplary projects for inspiration. If this plugin doesn't suit your needs you should definitely use one of the following 

[license-shield]: https://img.shields.io/github/license/github_username/repo.svg?style=flat-square
[license-url]: https://github.com/github_username/repo/blob/master/LICENSE.txt
[product-screenshot]: images/screenshot.png

