# Sinex - Learn Sign Language

Sinex is a static website for exploring introductory sign-language concepts. It combines lesson pages, common-gesture references, simple text and voice translators, a webcam-based gesture-detection demo, and a short interactive quiz.

## Features

- Introductory, advanced, and everyday-life lesson pages
- Visual references for **Hello**, **Thank You**, and **Please**
- Text-to-sign character translator
- Voice-to-sign character translator using the Web Speech API
- Webcam gesture-detection demo powered by TensorFlow.js Handpose
- Ten-question sign-language quiz with a score summary
- Responsive, dark-themed static interface

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Home page, tutorials, gesture gallery, and contact details |
| `basic.html` | Basic sign-language lesson page |
| `adv.html` | Advanced sign-language lesson page |
| `every.html` | Everyday sign-language lesson page |
| `trans.html` | Text-to-sign character translator |
| `audio.html` | Voice-to-sign character translator |
| `scanner.html` | Webcam-based hand gesture demo |
| `quiz.html` | Interactive quiz |

## Run locally

No build process or package installation is required. Serve the project folder with any static web server, then open the local address in a browser.

For example, with Python installed:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

You can also deploy the files directly to any static hosting provider.

## Browser requirements

- An up-to-date Chromium-based browser is recommended.
- The voice translator requires a browser that supports the Web Speech API.
- The scanner requires camera permission and must be served from `localhost` or HTTPS; browsers block camera access from ordinary `file://` pages.
- Internet access is required for the CDN-hosted TensorFlow.js, Handpose, Bootstrap, and Swiper resources.

## Project structure

```text
.
|-- index.html          # Main landing page
|-- basic.html          # Basic lessons
|-- adv.html            # Advanced lessons
|-- every.html          # Everyday lessons
|-- trans.html          # Text translator
|-- audio.html          # Voice translator
|-- scanner.html        # Webcam gesture detection
|-- quiz.html           # Quiz
|-- styles.css          # Shared styles
|-- *.png, *.jpg, *.jpeg, *.webp, *.avif
|                       # Site images and visual assets
`-- CNAME               # Custom-domain configuration
```

## Notes

- The lesson pages currently contain placeholder YouTube embed URLs (`example-video...`). Replace these with actual video IDs before publishing lessons.
- The translator pages represent characters with hand emojis. They are a lightweight visual aid, not an authoritative representation of any complete sign language.
- The webcam detector uses simple landmark heuristics for a small set of gestures and is intended as a demonstration rather than a production-grade recognition system.

## Contact

For questions or support, email [sinex0808@gmail.com](mailto:sinex0808@gmail.com).

## License

No license file is currently included. Add one before reusing or distributing the project under defined terms.
