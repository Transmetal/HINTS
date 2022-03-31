<!-- PROJECT LOGO -->
<h3 align="center">HINTS</h3>

<p align="center">
 Human Intelligence Narrowing Tool Set
<br />




<!-- TABLE OF CONTENTS -->
<details open="open">
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
        <li><a href="#frontend">Frontend</a></li>
        <li><a href="#backend">Backend</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![HINTS][product-screenshot]](https://github.com/rustrose/HINTS)

HINTS is a CRUD tool for housing information gathered from public OSINT resources on individuals (HUMINT) and organizations (ORGINT)

Now including:
* React interface for CRUD tasks relating to entries
* Strapi CMS using sqlite by default for persistence
* Knowledge base full of OSINT resources based on the work of Michael Bazzel
* HUMINT entries currently include 30+ topics
* ORGINT entries currently include 50+ topics


A list of commonly used resources that I find helpful are listed in the acknowledgements.

### Built With

* [Bootstrap](https://getbootstrap.com)
* [React](https://reactjs.org/)
* [Strapi](https://strapi.io/)
* [Python3](https://www.python.org/)



<!-- GETTING STARTED -->
## Getting Started

While running, this application houses an administrative interface at http://localhost:1337

The HINTS web interface can be found at http://localhost:3000

These sections both need to be running in order for things to work smoothly. It is recommended to utilize two seperate terminal windows for this however is most comfortable. 

### Prerequisites

Clone the repo
   ```sh
   git clone https://github.com/Transmetal/HINTS
   ```

### Frontend

1. Move into frontend directory
   ```sh
   cd HINTS/frontend/
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Run React frontend
   ```sh
   npm start develop
   ```


### Backend

1. Move into backend directory
   ```sh
   cd HINTS/backend/
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Run Strapi backend
   ```sh
   npm run develop
   ```
4. Set Admin User
5. Once logged in, browse to Settings under the General tab on the sidebar to the left
6. Next, browse to Roles under the Users & Permissions Plugin section
7. Select Public
8. Scroll down to permissions, find HUMINT, and select the "Select All" checkbox
9. Scroll up to the top of the page and save
10. Return to http://localhost:3000 and add a first entry

NOTE: Yes yes i know this is a worst practice. 
Soon the strapi JWT generation will be incorporated into the process to provide authorization. Soon...

Running the development mode makes troubleshooting far easier. This is still a work in progress.


<!-- ROADMAP -->
## Roadmap

* Exception Handling
* Input validation, formatting, and cleanup
* Facelift (I'm clearly a noob, help!)
* Better logo
* Image upload for entries
* Stabilize Ouroboros placement
* Generate reports from within web interface
* Proper authorization / authentication mechanism for each instance
* Docker installation

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
