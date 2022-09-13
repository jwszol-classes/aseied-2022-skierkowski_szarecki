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
[![Issues][issues-shield]][issues-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Measuring System</h3>

  <p align="center">
    Academic project at Gdansk University of Technology
    <br />
    <a href="https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    ·
    <a href="https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki/issues/new">Report Bug</a>
    ·
    <a href="https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki/issues/new">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
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
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
### Purpose
Analyze the data containing information on elevation variation by selecting groups of areas with the highest growth (continental North and South America). Elevation growth in a given location should be measured from at least 10 measurement points. Determine 6 groups of areas in relation to the average value of height increase. Please plot the detected areas on the map.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Built With

* ![Python3][Python.png]
* ![Pyspark][Pyspark.png]
* ![AWS][AWS.png]

### Technologies
The project site is an AWS cloud environment. 
We defined the following technology requirements on this environment:
* S3 cloud storage - source data ```s3://elevation-tiles-prod/```
* Cluster hardware configuration - m5.xlarge
* Cluster software configuration - JupyterEnterpriseGateway 2.1.0, Spark 2.4.8, Livy 0.7.1
* One node EMR cluster on AWS - EMR 5.36.0
### Dataset
In this project we used terrain-tiles dataset that is available via AWS resources.
It is a global dataset providing bare-earth terrain heights, tiled for easy usage and provided on S3.
Link to source dataset: </br>
[https://registry.opendata.aws/terrain-tiles/](https://registry.opendata.aws/terrain-tiles/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


---
<!-- GETTING STARTED -->
## Our solution

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## Results

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>


---
<!-- ROADMAP -->
## Roadmap

- [x] Downloading dataset from bucket & Creating PySpark Dataframe
- [x] Sorting tiles in Dataframe
- [x] Changing the color scale of downloaded tiles
- [x] Calculating gradient for each tile
- [x] Grouping tiles for 6 height growth groups 
- [x] Combination of all tiles
- [x] Coloring and presenting North and South America

See the [open issues](https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Names:
* Lukasz Szarecki
* Marcel Skierkowski

Project Link: [https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki](https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- Links -->
## Links

* https://spark.apache.org/docs/latest/api/python/reference/ 
* https://sparkbyexamples.com/pyspark/


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/jwszol-classes/aseied-2022-skierkowski_szarecki.svg?style=for-the-badge
[contributors-url]: https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/jwszol-classes/aseied-2022-skierkowski_szarecki.svg?style=for-the-badge
[stars-shield]: https://img.shields.io/github/stars/jwszol-classes/aseied-2022-skierkowski_szarecki.svg?style=for-the-badge
[stars-url]: https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki/stargazers
[issues-shield]: https://img.shields.io/github/issues/jwszol-classes/aseied-2022-skierkowski_szarecki.svg?style=for-the-badge
[issues-url]: https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki/issues
[license-shield]: https://img.shields.io/github/license/jwszol-classes/aseied-2022-skierkowski_szarecki.svg?style=for-the-badge
[license-url]: https://github.com/jwszol-classes/aseied-2022-skierkowski_szarecki/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png
[Python.png]: https://www.python.org/static/community_logos/python-powered-w-100x40.png
[Pyspark.png]: images/pyspark.png
[AWS.png]: images/aws.png