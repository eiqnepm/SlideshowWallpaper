<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



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
[![GPL v3][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">

<h3 align="center">Slideshow Wallpaper</h3>
  
  <p align="center"><a href='https://play.google.com/store/apps/details?id=io.github.doubi88.slideshowwallpaper'><img height="80" alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png'/></a>
<a href="https://f-droid.org/packages/io.github.doubi88.slideshowwallpaper">
    <img src="https://fdroid.gitlab.io/artwork/badge/get-it-on.png"
    alt="Get it on F-Droid"
    height="80">
</a>
  </p>
  <p align="center">
    A Live Wallpaper for Android, displaying user selected images.
    <br />
    <a href="https://github.com/doubi88/SlideshowWallpaper"><strong>Explore the sources »</strong></a>
    <br />
    <br />
    <a href="https://github.com/doubi88/slideshowwallpaper/issues">Report Bug</a>
    ·
    <a href="https://github.com/doubi88/slideshowwallpaper/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#project-license">Project License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#about-this-readme">About this README</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

Slideshow Wallpaper is a Live Wallpaper for Android, that displays a slideshow of user selected images. You can customize the duration, how long the images are displayed, the order and the display mode. Separate image lists can be configured for Android's light and dark themes; the wallpaper switches lists with the system theme.

<img src="docs/images/screenshot.png" height="605">

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Manual signed APK releases

The **Manual signed APK release** GitHub Actions workflow builds an optimized
release APK, verifies its signature, and creates a timestamped prerelease with
the APK, its SHA-256 checksum, and a GitHub build-provenance attestation. The
workflow must be merged to the repository's default branch before GitHub makes
it available for manual dispatch from the Actions tab. When running it, select
the branch or commit to build; each release points to that exact commit. Only
select a ref whose code you trust, because its Gradle build runs on the runner
while the signing keystore is present.

Before running it, add these repository Actions secrets under
**Settings → Secrets and variables → Actions**:

- `ANDROID_KEYSTORE_BASE64`: the signing keystore encoded as one line of
  Base64. For example, on Linux, run `base64 -w 0 SlideshowWallpaper.jks`.
- `ANDROID_KEYSTORE_PASSWORD`: the keystore password.
- `ANDROID_KEY_ALIAS`: the signing key alias.
- `ANDROID_KEY_PASSWORD`: the signing key password.

Use the same signing key as prior releases if users need to install this APK as
an update. Keep a secure backup of that key; without it, future APKs cannot be
signed as the same publisher. The keystore is written only on the GitHub-hosted
runner and is not committed to the repository.

The checksum detects changes to the downloaded APK. The attestation can be
verified with GitHub CLI, for example:
`gh attestation verify SlideshowWallpaper-<timestamp>.apk --repo eiqnepm/SlideshowWallpaper`.
It ties the APK to the GitHub Actions workflow and source commit; it does not
by itself prove that the source code is safe. Review the source and workflow
for the attested commit before trusting a release.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- LICENSE -->
## Project License

Distributed under GPL v3. See [`LICENSE`][license-url] for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Doubi88 - tobis_mail@yahoo.de\
(see https://github.com/Doubi88/.github/blob/master/CONTACT.md)

Project Link: [https://github.com/doubi88/slideshowwallpaper](https://github.com/doubi88/slideshowwallpaper)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## About this README
This README file was created from the [Best README Template](https://github.com/othneildrew/Best-README-Template).

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[android-studio-url]: https://developer.android.com/studio
[contributors-shield]: https://img.shields.io/github/contributors/doubi88/slideshowwallpaper.svg?style=for-the-badge
[contributors-url]: https://github.com/doubi88/slideshowwallpaper/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/doubi88/slideshowwallpaper.svg?style=for-the-badge
[forks-url]: https://github.com/doubi88/slideshowwallpaper/network/members
[stars-shield]: https://img.shields.io/github/stars/doubi88/slideshowwallpaper.svg?style=for-the-badge
[stars-url]: https://github.com/doubi88/slideshowwallpaper/stargazers
[issues-shield]: https://img.shields.io/github/issues/doubi88/slideshowwallpaper.svg?style=for-the-badge
[issues-url]: https://github.com/doubi88/slideshowwallpaper/issues
[license-shield]: https://img.shields.io/github/license/doubi88/slideshowwallpaper.svg?style=for-the-badge
[license-url]: https://github.com/doubi88/slideshowwallpaper/blob/master/LICENSE
