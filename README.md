<!-- taken from Best-README-Template
<!-- https://github.com/othneildrew/Best-README-Template
<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![GNU GPL v3 License][license-shield]][license-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h3 align="center">IntelliFreeze</h3>

  <p align="center">
    Intelligently freeze entire groups and folders of tracks within REAPER
    <br />
    <a href="https://github.com/Timtam/IntelliFreeze/issues">Report Bug</a>
    �
    <a href="https://github.com/Timtam/IntelliFreeze/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
* [Usage](#usage)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)



<!-- ABOUT THE PROJECT -->
## About The Project

With a collaboration on the horizon, I started to check my possible ways to freely share work with others without having to re-import tracks all the time, but also allowing me and my collaborators to use plug-ins that the others don't have. Freezing was deffinetily the way to go, but my templates usually work with multiple levels of track folders and freezing a folder would just create a frozen item and mute all sub-tracks, which would cause various issues for my collaborators. Why not freeze all tracks individually from the get-go?

Thats exactly how the actions within this script work, they check the currently selected tracks, recursively gather all the sub-tracks that require freezing and freeze them individually bottom-up.

### Built With

* [Lua 5.3](https://www.lua.org/manual/5.3/)
* [REAPER 6.53 and above (older versions might run as well)](https://reaper.fm)

<!-- GETTING STARTED -->
## Getting Started

### Installation

#### ReaPack

It is recommended to get the latest stable version from ReaPack by synchronizing your repositories and searching for IntelliFreeze in the package list. This will make sure to add all the available actions to your actions list as well.

#### Building from source

##### Clone

If you thus instead want to test the bleeding edge build of this package, clone this repository locally:

```sh
git clone https://github.com/Timtam/IntelliFreeze.git
```

Copy the timtam_IntelliFreeze folder into your REAPER's scripts folder afterwards.

note: make sure to copy the folder directly into your Scripts folder, not in some other sub-folder or a totally different directory to make sure that the scripts work directly.

##### Adding actions

Open an empty project within REAPER and open the actions list (shortcut: F4).
Now select New Action and Load ReaScript. Make sure to load every timtam_IntelliChords file from within the timtam_IntelliFreeze folder, except the one that is called timtam_IntelliFreeze.lua. That one only contains dependencies and doesn't contain any action.

## Usage

Its as easy as it can get, just select the tracks, folders, whatever you want to freeze within REAPER and run the corresponding action from the actions list. Feel free to bind them to keystrokes if you end up using them often.

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/Timtam/IntelliFreeze/issues) for a list of proposed features (and known issues).

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

### Contribute by coding

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Contribute by testing

Feel free to give these scripts a go and see if they fit your workflow.
Do you like those scripts, but can think of a way they might become even more useful to you? Feel free to let me know by opening an issue or contacting me via email at <software@satoprogs.de>.
Same goes for bugs you might have encountered or new features you'd like to see.

### Contribute by paying me a coffee

Developing takes time and effort and since those scripts are free to use and open-source, I don't get anything out of it except appreciation. Appreciation doesn't pay monthly bills though. 
If you think those scripts greatly improved your life by helping you with your productivity and workflow, or you simply want to give something back, i'd greatly appreciate a small donation via PayPal to the following link: <https://paypal.me/ToniRonaldBarth>
Don't feel obligated though.

<!-- LICENSE -->
## License

Distributed under the GNU GPL v3 License. See `LICENSE` for more information.

<!-- CONTACT -->
## Contact

Toni Barth - [@GixGax95](https://twitter.com/GixGax95) - software@satoprogs.de

Project Link: [https://github.com/Timtam/IntelliFreeze](https://github.com/Timtam/IntelliFreeze)



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Timtam/IntelliFreeze.svg?style=flat-square
[contributors-url]: https://github.com/Timtam/IntelliFreeze/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Timtam/IntelliFreeze.svg?style=flat-square
[forks-url]: https://github.com/Timtam/IntelliFreeze/network/members
[stars-shield]: https://img.shields.io/github/stars/Timtam/IntelliFreeze.svg?style=flat-square
[stars-url]: https://github.com/Timtam/IntelliFreeze/stargazers
[issues-shield]: https://img.shields.io/github/issues/Timtam/IntelliFreeze.svg?style=flat-square
[issues-url]: https://github.com/Timtam/IntelliFreeze/issues
[license-shield]: https://img.shields.io/github/license/Timtam/IntelliFreeze.svg?style=flat-square
[license-url]: https://github.com/Timtam/IntelliFreeze/blob/master/LICENSE
