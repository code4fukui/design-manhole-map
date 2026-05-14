# Design Manhole Map

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

[
![View Demo](https://img.shields.io/badge/View%20Demo-GitHub%20Pages-2ea44f?style=for-the-badge)
](https://eiichimiyagawa.github.io/design-manhole-map/)

An interactive web map showcasing the unique and artistic "design manhole" covers found across Japan.

## Demo

Explore the live map here:
**[https://eiichimiyagawa.github.io/design-manhole-map/](https://eiichimiyagawa.github.io/design-manhole-map/)**

Click on a marker to view details about a specific manhole cover, including its location, a photo, and a description of its design.

## Features

- **Interactive Map:** Pan and zoom across Japan to find design manhole covers.
- **Detailed Popups:** Click any marker to see the manhole's name, address, coordinates, and description.
- **High-Quality Images:** View a photo of each manhole cover's unique design directly on the map.
- **Open Data:** All location data is available in a simple, accessible CSV format.

## Technology Stack

- **[OpenLayers](https://openlayers.org/):** Powers the interactive map functionality.
- **[CSV.js](https://github.com/code4fukui/CSV.js):** Used for fetching and parsing the manhole data from the CSV file.
- **HTML/CSS/JavaScript:** The core web technologies used to build the application.

## Running Locally

To run this project on your local machine, you must serve the files from a local web server. This is necessary because browser security policies (CORS) prevent web pages from loading local files directly.

**Prerequisites:**
- [Node.js](https://nodejs.org/) (to use `npx`)

**Steps:**

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/eiichimiyagawa/design-manhole-map.git
    cd design-manhole-map
    ```

2.  **Start a local server:**
    A simple way is to use the `http-server` package via `npx`.
    ```sh
    npx http-server
    ```

3.  **Open in your browser:**
    Navigate to the URL provided by the server (e.g., `http://127.0.0.1:8080`).

## Data Source

The manhole cover data is available as a CSV file and is sourced from the Sewage Publicity Platform.

- **Open Data CSV:** [design-manhole-map/data.csv](https://eiichimiyagawa.github.io/design-manhole-map/data.csv)
- **Original Source:** [Manhole Card Search | Sewage Publicity Platform](https://www.gk-p.jp/mhcard/?pref=18#mhcard_result)

## License

MIT License — see [LICENSE](LICENSE).