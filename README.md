# Finder Services

Quick Actions for the macOS Finder, mostly for type designers and font folks. Each service lives in its own folder with its own README and `install.sh`.

| Service | What it does |
|---|---|
| [Trim Image to Content](Trim%20Image%20to%20Content) | Crops images to their content, using the top left pixel as the background color. |

## Install a service

Clone this repository, then run the `install.sh` in the service’s folder. It copies the `.workflow` into `~/Library/Services`. The service then shows up in Finder under right-click > Quick Actions (and may need enabling in System Settings > Extensions > Finder).

## License

Apache License 2.0, see [LICENSE](LICENSE).
