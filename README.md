<h2 align="center">
    <br>
    青鸾 Qingluan — HTTPie CLI (community revival)
    <br>
    Human-friendly HTTP client for the API era
</h2>

<p align="center">
  <a href="#why-qingluan">Why Qingluan</a> •
  <a href="#revival-status">Revival status</a> •
  <a href="#installation">Installation</a> •
  <a href="#usage">Usage</a> •
  <a href="#contributing">Contributing</a> •
  <a href="#acknowledgments">Acknowledgments</a>
</p>

---

**Why Qingluan (青鸾)?** In Chinese legend, the qingluan is the divine messenger bird of the Queen Mother of the West — the bird that carries letters. An HTTP client is exactly that: a messenger that carries your requests and brings back answers. The name honors the tool's essence.

This is a **community revival** of the [HTTPie CLI](https://github.com/httpie/cli) — the human-friendly command-line HTTP client for the API era, with intuitive syntax, JSON support, sessions, downloads, and plugins.

The upstream project has been effectively dormant: the last commit to `main` was December 2024, the last release 3.2.4 shipped November 2024, and **176 pull requests** (with more arriving weekly) sat unreviewed. The community never stopped contributing — the maintainers stopped responding. This repository continues that work.

## Revival status

- **Fork basis**: upstream `main` at `5b604c37` (2024-12-17), preserving full history and the original BSD 3-Clause license.
- **Triage**: all 176 open pull requests were reviewed and triaged; same-problem clusters are being merged into the best implementation, security fixes land first.
- **Upstream invitation**: every PR and issue author is invited to bring their original PR/issue number here — see [ACKNOWLEDGMENTS.md](ACKNOWLEDGMENTS.md) for the full honor roll.
- The original README is preserved at [docs/README-upstream.md](docs/README-upstream.md).

## Installation

```bash
# pip
pip install httpie

# pipx (recommended for CLI tools)
pipx install httpie

# macOS
brew install httpie

# Windows
choco install httpie
```

## Usage

```bash
# GET
http GET httpie.io

# POST with JSON
http POST api.example.com/users name=John email=john@example.com

# Sessions, downloads, auth and more
http --session=github --download GET api.example.com/releases/latest
```

See the original documentation in [`docs/`](docs/) for the full feature set.

## Contributing

**Coming from upstream?** Bring your original PR or issue number — triaged contributions are prioritized. Security fixes land first. See [CONTRIBUTING.md](CONTRIBUTING.md) and the [acknowledgments page](ACKNOWLEDGMENTS.md).

## Acknowledgments

This revival is carried by the upstream community: [137 pull request authors](ACKNOWLEDGMENTS.md) and [165 issue authors](ACKNOWLEDGMENTS.md) with open work at fork time are honored by name, alongside all 1,200+ historical contributors.

## License

BSD 3-Clause — see [LICENSE](LICENSE). Original copyright © 2012-2022 Jakub Roztocil and upstream contributors, preserved in [NOTICE](NOTICE).
