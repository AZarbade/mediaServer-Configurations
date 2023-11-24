# Dockerized Media-Server Environment

## Overview

This project sets up a Dockerized environment with multiple services for home media server purposes. It includes services like a homepage, Flaresolverr for solving challenges from protected websites, Jellyfin for media streaming, Prowlarr for managing your media library, qBittorrent for torrenting, Sonarr and Radarr for managing your TV shows and movies, Jellyseerr for handling media metadata, and Speedtest-Tracker for monitoring network speed.

## Getting Started

Follow these steps to set up and run the project on your local machine.

### Prerequisites

Make sure you have the following software installed:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/your-repo.git
    cd your-repo
    ```

2. Update the configuration in the `docker-compose.yml` file:

    - Adjust `data_path` and `config_path` in the `x-common-vars` section if needed.
    - Configure each service's settings as required.

3. Run the following command to start the services:

    ```bash
    docker-compose up -d
    ```

### Accessing Services

- **Homepage:** [http://localhost:3000](http://localhost:3000)
  - A customizable homepage for your needs.
- **Flaresolverr:** [http://localhost:8191](http://localhost:8191)
  - A service for solving challenges from protected websites.
- **Jellyfin:** [http://localhost:8096](http://localhost:8096)
  - Media streaming server.
- **Prowlarr:** [http://localhost:9696](http://localhost:9696)
  - Media library manager.
- **qBittorrent:** [http://localhost:8080](http://localhost:8080)
  - Torrent client for downloading and managing torrents.
- **Sonarr:** [http://localhost:8989](http://localhost:8989)
  - TV show management.
- **Radarr:** [http://localhost:7878](http://localhost:7878)
  - Movie management.
- **Jellyseerr:** [http://localhost:5055](http://localhost:5055)
  - Handles metadata for media.
- **Speedtest-Tracker:** [http://localhost:9090](http://localhost:9090)
  - Monitors network speed.

## Configuration

Adjust the configuration options in the `docker-compose.yml` file to suit your requirements.

### Common Variables

- `data_path`: Path for data storage.
- `config_path`: Path for configuration files.

## License

This project is licensed under the [MIT License](LICENSE.md).
