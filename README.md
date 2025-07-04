# podcast:location Tag Demo

This is a demo implementation of the [`podcast:location`](https://podcasting2.org/docs/podcast-namespace/tags/location) tag, part of the Podcast Namespace initiative. It provides a simple, user-friendly interface for podcast hosting platforms to help creators specify the **location of a podcast**: such as where it was made (`creator`) and/or what it is about (`subject`).

---

## About This Demo

This implementation of the `podcast:location` tag follows the latest specifications and best practices, including the use of OpenStreetMap (OSM) and OSM IDs. A key goal of this demo is to provide location autocompletion to improve user experience and data accuracy.

The official free OSM API imposes strict rate limits and does not support autocomplete functionality. Although it is technically possible to self-host an OSM instance with autocomplete support, doing so requires considerable infrastructure and maintenance overhead. For this reason, this demo uses [a third-party provider built on OSM data](https://locationiq.com) that offers more flexibility and reliable autocompletion out of the box.

While podcast hosting companies may design their own UI/UX, the core behavior demonstrated here is intended as a reference for implementing the tag properly. For instance, including the location type (such as “City”, "Neighborhood", “Mall”, or “Winery”) next to autocomplete results is strongly recommended to aid disambiguation and ensure data accuracy.

---

## ⚠️ Disclaimer

This is a quick proof of concept (not optimized for mobile) built to demonstrate the core logic and UX behind the `podcast:location` tag.

The entire demo, including HTML, CSS, and JavaScript, is contained in a **single HTML file** to make it self-contained and easy to share. The focus is not on the code itself (which was kept intentionally frugal), but on the overall user interface logic and behavior it demonstrates.

🔑 The live demo includes a **public API key** connected to a free account with daily rate limits. To state the obvious, this is **NOT** best practice: the key should be kept on a secure backend. We left it visible on purpose to keep the GitHub Pages demo fully functional. Please do not abuse the key with excessive requests.

---

## 🚀 Live Demo

[https://your-username.github.io/podcast-location-demo](https://your-username.github.io/podcast-location-demo)

---

## License

[MIT](LICENSE)
