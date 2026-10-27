# Zelu Landing Page

[![Swift](https://img.shields.io/badge/Swift-5.9-F05138?logo=swift&logoColor=white)](https://swift.org)
[![Ignite](https://img.shields.io/badge/Ignite-static%20site-000000)](https://github.com/twostraws/Ignite)
[![GitHub Pages](https://img.shields.io/badge/deploy-GitHub%20Pages-222222?logo=githubpages&logoColor=white)](https://zelu.online)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

The marketing site for the [Zelu](https://github.com/EnzoFerroni/Zelu) iOS app, written in Swift with the Ignite static site generator and live at **[zelu.online](https://zelu.online)**.

## Table of Contents

- [About](#about)
- [Sections](#sections)
- [Built With](#built-with)
- [Getting Started](#getting-started)
- [Deployment](#deployment)
- [Project Structure](#project-structure)
- [Team](#team)
- [License](#license)

## About

Zelu helps people keep their friendships alive by turning each friend into a bubble
that grows when you meet and drifts into the void when you don't. This site presents
the app, explains how it works and sends visitors to the App Store. Every page is
described in Swift and compiled to static HTML, so the site needs no server or
JavaScript framework. The copy is in Portuguese.

## Sections

- **Hero** with the App Store link
- **Features**: friends in orbit, adding by proximity, meeting goals, moments and
  rescuing friends from the void
- **FAQ**: what Zelu is, how to add a friend, why no account is needed and how
  meetings are detected
- **Footer** with Instagram and TikTok links
- Scroll-driven animations in a small vanilla `app.js`

## Built With

- [Ignite](https://github.com/twostraws/Ignite) by Paul Hudson: pages, components and
  layouts written in Swift
- Custom CSS and Google Fonts
- GitHub Actions to build and publish to GitHub Pages

## Getting Started

Requirements: Xcode 15 or later (Swift 5.9) on macOS.

```bash
git clone https://github.com/EnzoFerroni/zelu-landing.git
cd zelu-landing
swift run
```

The site is generated into `Build/`. To preview it, install the
[Ignite CLI](https://github.com/twostraws/IgniteCLI) and run `ignite run --preview`,
or serve the folder with any static server.

## Deployment

Every push to `main` runs `.github/workflows/deploy.yml`, which builds the site with
`swift run` on a macOS runner and publishes `Build/` to GitHub Pages. The custom domain
is set by `Assets/CNAME`. The production site is deployed from the team repository
[C13G1/zelu-landing](https://github.com/C13G1/zelu-landing); this fork does not
publish Pages.

## Project Structure

```
├── Sources/
│   ├── Site.swift           Site configuration (name, URL, layout)
│   ├── Pages/Home.swift     The landing page
│   ├── Components/          NavBar, Hero, Features, Faq, Footer
│   ├── Layouts/             MainLayout
│   └── Content.swift        Copy for features and FAQ
├── Assets/                  CSS, JavaScript, images and CNAME
└── .github/workflows/       Build and deploy to GitHub Pages
```

## Team

<div align="center">
  <table>
    <tr>
      <td align="center" width="25%">
        <a href="https://github.com/camilatoniato"><img src="https://github.com/camilatoniato.png" width="90" alt="Camila Toniato"/></a>
        <br/><sub><b>Camila Toniato</b></sub><br/><br/>
        <a href="https://github.com/camilatoniato"><img src="https://skillicons.dev/icons?i=github" alt="GitHub"/></a>
        <a href="https://www.linkedin.com/in/camila-ruiz-toniato-91a926301/"><img src="https://skillicons.dev/icons?i=linkedin" alt="LinkedIn"/></a>
      </td>
      <td align="center" width="25%">
        <a href="https://github.com/dayoleal"><img src="https://github.com/dayoleal.png" width="90" alt="Dayô Araújo"/></a>
        <br/><sub><b>Dayô Araújo</b></sub><br/><br/>
        <a href="https://github.com/dayoleal"><img src="https://skillicons.dev/icons?i=github" alt="GitHub"/></a>
        <a href="https://www.linkedin.com/in/dayo-araujo/"><img src="https://skillicons.dev/icons?i=linkedin" alt="LinkedIn"/></a>
      </td>
      <td align="center" width="25%">
        <a href="https://github.com/EnzoFerroni"><img src="https://github.com/EnzoFerroni.png" width="90" alt="Enzo Ferroni"/></a>
        <br/><sub><b>Enzo Ferroni</b></sub><br/><br/>
        <a href="https://github.com/EnzoFerroni"><img src="https://skillicons.dev/icons?i=github" alt="GitHub"/></a>
        <a href="https://www.linkedin.com/in/enzoferroni/"><img src="https://skillicons.dev/icons?i=linkedin" alt="LinkedIn"/></a>
      </td>
      <td align="center" width="25%">
        <a href="https://github.com/JonasFNMelo"><img src="https://github.com/JonasFNMelo.png" width="90" alt="Jonas Melo"/></a>
        <br/><sub><b>Jonas Melo</b></sub><br/><br/>
        <a href="https://github.com/JonasFNMelo"><img src="https://skillicons.dev/icons?i=github" alt="GitHub"/></a>
        <a href="https://www.linkedin.com/in/jonas-melo-/"><img src="https://skillicons.dev/icons?i=linkedin" alt="LinkedIn"/></a>
      </td>
    </tr>
    <tr>
      <td align="center" width="25%">
        <a href="https://github.com/mathicastanha"><img src="https://github.com/mathicastanha.png" width="90" alt="Mathias Castanha"/></a>
        <br/><sub><b>Mathias Castanha</b></sub><br/><br/>
        <a href="https://github.com/mathicastanha"><img src="https://skillicons.dev/icons?i=github" alt="GitHub"/></a>
        <a href="https://www.linkedin.com/in/mathias-castanha/"><img src="https://skillicons.dev/icons?i=linkedin" alt="LinkedIn"/></a>
      </td>
      <td align="center" width="25%">
        <a href="https://github.com/ThomasPGR"><img src="https://github.com/ThomasPGR.png" width="90" alt="Thomas Pinheiro Grandin"/></a>
        <br/><sub><b>Thomas Pinheiro Grandin</b></sub><br/><br/>
        <a href="https://github.com/ThomasPGR"><img src="https://skillicons.dev/icons?i=github" alt="GitHub"/></a>
        <a href="https://www.linkedin.com/in/thomas-pinheiro-grandin-704bb6297/"><img src="https://skillicons.dev/icons?i=linkedin" alt="LinkedIn"/></a>
      </td>
    </tr>
  </table>
</div>

Part of [Zelu](https://github.com/EnzoFerroni/Zelu), built at the Apple Developer Academy | Mackenzie.

## License

Released under the [MIT License](LICENSE). Copyright (c) 2026 the Zelu team: Camila
Toniato, Dayô Araújo, Enzo Ferroni, Jonas Melo, Mathias Castanha and Thomas Pinheiro
Grandin. Based on
the IgniteStarter template, copyright (c) 2024 Paul Hudson and other authors.
