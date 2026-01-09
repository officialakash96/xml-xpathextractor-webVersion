# XML XPath Extractor - GitHub Pages Version

This is a pure client-side JavaScript version of the XML XPath Extractor that can be hosted on GitHub Pages.

## Features

- ✅ Pure HTML/CSS/JavaScript (no backend required)
- ✅ Works entirely in the browser
- ✅ CORS proxy support for fetching external XML feeds
- ✅ All features from the original Flask version
- ✅ Can be hosted on GitHub Pages

## CORS Considerations

Since this version runs entirely in the browser, it uses a CORS proxy service (allorigins.win) to fetch XML feeds that don't allow direct cross-origin requests. This works for most public XML feeds.

## Local Testing

To test locally, simply open `index.html` in a web browser, or use a local server:

```bash
# Python 3
python3 -m http.server 8000

# Then open http://localhost:8000 in your browser
```

## Files

- `index.html` - Complete standalone application
- `LI-Logo.png` - LinkedIn logo
- `README.md` - This file

## Differences from Flask Version

1. **CORS proxy**: Uses allorigins.win to fetch XML feeds
2. **No server**: Runs entirely in the browser
3. **Same features**: All XPath extraction, attribute display, copy functionality, etc.
4. **Same UI**: Identical design and user experience

## Author

Designed by [Akash Singh](https://www.linkedin.com/in/akashsinghjsr/)

## License

© 2026 XML XPath Extractor
