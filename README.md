# Loom-ish — a free, open-source Loom alternative

<p align="center">
  <img src="./logo-144.png" width="96" height="96" alt="Loom-ish logo">
</p>

[Loom-ish](https://loomalt.leontang.ca/) is a private browser screen recorder for capturing your screen, webcam, and microphone without creating an account or uploading the recording to a hosted video library.

Recording and editing happen in your browser. When you finish, you must download and save the video to your own device because Loom-ish does not store a copy.

## Why Loom-ish?

- Free and open source
- No account or installation
- No video uploads or hosted storage
- Screen, tab, webcam, and microphone recording
- Configurable webcam bubble
- 720p, 1080p, and original-resolution options
- Built-in trimming and playback-speed editing
- Local MP4 or WebM download, depending on browser support

## Try it

Use the live recorder at **[loomalt.leontang.ca](https://loomalt.leontang.ca/)**.

Chrome and Edge provide the fullest experience, including the floating webcam bubble. Other modern desktop browsers may support recording with fewer controls.

## Privacy model

Loom-ish uses browser screen-share, camera, and microphone APIs directly. The recording is assembled locally in the browser and is not sent to the Loom-ish server.

Because there is no hosted video storage, closing or refreshing the page before downloading can permanently lose the recording.

## Run locally

Clone the repository and serve its root directory with any static web server:

```bash
git clone https://github.com/Ltang909/loom-ish.git
cd loom-ish
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

Camera and screen-capture permissions generally require HTTPS or localhost.

## Deploy

The project is a static website with no build step or server-side dependencies. Deploy every file in the repository root to the document root for `loomalt.leontang.ca`.

Important files:

- `index.html` — recorder, editor, visible SEO content, and structured data
- `robots.txt` — crawler permissions and sitemap reference
- `sitemap.xml` — canonical URL submitted to search engines
- `llms.txt` — concise product facts for compatible AI systems
- `logo.png` — high-resolution transparent brand mark
- `logo-144.png` — optimized header asset
- `favicon-32.png` and `apple-touch-icon.png` — browser and device icons

## Support

For support inquiries, email [leon@leontang.ca](mailto:leon@leontang.ca).

## Contributing

Bug reports and focused improvements are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Licensed under the [MIT License](LICENSE).

Loom-ish is an independent project and is not affiliated with Loom or Atlassian.
