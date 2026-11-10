<a id="readme-top"></a>

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![Tampermonkey][tampermonkey-shield]][tampermonkey-url]

<br />
<div align="center">
  <h3 align="center">Reddit Unfollow All</h3>

  <p align="center">
    A userscript that unsubscribes you from all subreddits in bulk, with a draggable control panel and configurable speed.
    <br />
    <a href="https://github.com/aybrkaknc/RedditUnfollowAllScript"><strong>Explore the repository</strong></a>
    <br />
    <br />
    <a href="https://github.com/aybrkaknc/RedditUnfollowAllScript/issues/new?labels=bug">Report Bug</a>
    &middot;
    <a href="https://github.com/aybrkaknc/RedditUnfollowAllScript/issues/new?labels=enhancement">Request Feature</a>
  </p>

  <p align="center">
    <a href="README.md">English</a> | <a href="README.tr.md">Türkçe</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#technical-notes">Technical Notes</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## About The Project

Reddit Unfollow All automates the process of unsubscribing from Reddit subreddits. It adds a non-intrusive overlay to the subreddit list page and runs the unsubscribe actions one by one, with a speed preset that helps avoid rate limiting.

- **UI Overlay**: Draggable panel with Minimize and Close controls.
- **Throttling Control**: Preset execution intervals from 200ms to 1500ms.
- **State Management**: Shows total and remaining counts and an execution log inside the panel.
- **I18n Engine**: Detects the browser language automatically (English and Turkish).
- **Selector Engine**: Works with both legacy (`old.reddit.com`) and modern Reddit DOM structures.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* [![JavaScript][JavaScript-shield]][JavaScript-url]
* [![Tampermonkey][Tampermonkey-badge]][Tampermonkey-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Getting Started

Follow these steps to run the script in your browser.

### Prerequisites

* A userscript manager such as Tampermonkey
  ```
  Chrome, Edge, Firefox, Safari and others: https://www.tampermonkey.net/
  ```

### Installation

1. Install [Tampermonkey](https://www.tampermonkey.net/) in your browser.
2. Create a new script in Tampermonkey.
3. Copy the contents of [`betik.js`](betik.js) and paste them into the new script.
4. Save the script and make sure it is enabled.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage

1. Open [https://www.reddit.com/subreddits/](https://www.reddit.com/subreddits/) (or `old.reddit.com/subreddits/`).
2. Wait for the control panel to appear in the page.
3. Choose a speed preset. "Normal" or "Slow" is recommended for large subscription lists.
4. Click "START" to begin. Use "PAUSE" and "RESUME" to control the process.
5. Drag the panel by its header to reposition it.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Technical Notes

The script performs batch DOM interactions on the subreddit page. Use a slower preset for large lists to keep requests stable. Keep the page open until the process completes.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contributing

Contributions are welcome. If you have a suggestion that would make this better, fork the repository and create a pull request, or open an issue with the tag "enhancement".

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contact

Ayberk - [@aybrkaknc](https://github.com/aybrkaknc)

Project Link: [https://github.com/aybrkaknc/RedditUnfollowAllScript](https://github.com/aybrkaknc/RedditUnfollowAllScript)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Acknowledgments

* [Best-README-Template](https://github.com/aybrkaknc/Best-README-Template)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/aybrkaknc/RedditUnfollowAllScript.svg?style=for-the-badge
[contributors-url]: https://github.com/aybrkaknc/RedditUnfollowAllScript/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/aybrkaknc/RedditUnfollowAllScript.svg?style=for-the-badge
[forks-url]: https://github.com/aybrkaknc/RedditUnfollowAllScript/network/members
[stars-shield]: https://img.shields.io/github/stars/aybrkaknc/RedditUnfollowAllScript.svg?style=for-the-badge
[stars-url]: https://github.com/aybrkaknc/RedditUnfollowAllScript/stargazers
[issues-shield]: https://img.shields.io/github/issues/aybrkaknc/RedditUnfollowAllScript.svg?style=for-the-badge
[issues-url]: https://github.com/aybrkaknc/RedditUnfollowAllScript/issues
[tampermonkey-shield]: https://img.shields.io/badge/userscript-Tampermonkey-00485B?style=for-the-badge
[tampermonkey-url]: https://www.tampermonkey.net/
[JavaScript-shield]: https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black
[JavaScript-url]: https://developer.mozilla.org/en-US/docs/Web/JavaScript
[Tampermonkey-badge]: https://img.shields.io/badge/Tampermonkey-00485B?style=for-the-badge
[Tampermonkey-url]: https://www.tampermonkey.net/
