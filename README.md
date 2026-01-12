# XML XPath Extractor - GitHub Pages Version

A pure client-side JavaScript version of the XML XPath Extractor that works entirely in your browser - no backend or server required!

## Features

- ✅ **Pure HTML/CSS/JavaScript** - No backend, no installation needed
- ✅ **Works entirely in the browser** - Just open and use
- ✅ **Smart path formatting** - Simple paths when no attributes, double slash format when attributes present
- ✅ **Optimized performance** - Processes only first instance of repeating elements for faster extraction
- ✅ **Sample values** - Displays actual values from the XML feed
- ✅ **Full scrolling support** - View all XPaths without cutoff
- ✅ **CORS proxy support** - Fetches external XML feeds that don't allow direct cross-origin requests
- ✅ **Authentication support** - Basic auth for password-protected feeds
- ✅ **Copy to clipboard** - Easy XPath copying
- ✅ **Collapsible elements** - Parent-child hierarchy with expand/collapse
- ✅ **Can be hosted on GitHub Pages** - Free hosting with GitHub

## Getting Started (For Beginners)

### Run Locally on Your Computer

If you want to run it on your own computer or make changes:

#### Prerequisites

You only need **Git** installed on your computer:
- Check if Git is installed: Open Terminal (Mac/Linux) or Command Prompt (Windows) and run:
  ```bash
  git --version
  ```
- If not installed, download from: https://git-scm.com/downloads

#### Step 1: Clone the Repository

Open your Terminal (Mac/Linux) or Command Prompt (Windows) and run:

```bash
# Navigate to where you want to store the project
cd ~/Documents

# Clone the repository
git clone https://github.com/akasingh_LinkedIn/xml-xpath-extractor.git

# Enter the project directory
cd xml-xpath-extractor
```

#### Step 2: Open in Browser

You have two options to run it locally:

**Option A: Using Python (if you have Python installed)**

```bash
# Python 3
python3 -m http.server 8080

# Then open http://localhost:8080 in your browser
```

**Option B: Simply Open the HTML File**

Just double-click the `index.html` file in the folder, and it will open in your browser!

Note: Some features like CORS proxy might work better with a local server (Option A).

🎉 **You're ready to use the XPath Extractor!**

#### Step 3: Stop the Server (if using Python)

When you're done, press `Ctrl+C` in the terminal to stop the server.

## How to Use the Application

1. **Enter XML Feed URL**: Paste your XML feed URL in the input field
2. **Optional Authentication**: If your feed requires a username/password, expand the "Authentication (Optional)" section
   - Note: Some password-protected feeds may be blocked by browser CORS policies. For those, use the [Flask backend version](https://github.com/akasingh_LinkedIn/xpath-extractor-python)
3. **Click "Extract XPaths"**: The app will fetch and parse the XML
4. **View Results**: All XPath expressions will be displayed with:
   - Sample values from the feed
   - Copy buttons for each XPath
   - Expandable child elements
   - Attributes (if present)
5. **Copy XPaths**: Click the "Copy" button next to any XPath to copy it to your clipboard
6. **Expand/Collapse**: 
   - Click on any XPath item to expand/collapse it
   - Use "Expand All" or "Collapse All" buttons for bulk actions

## Example XML Feed URLs to Test

Try these sample feeds to test the application:

- **Job Feed**: `https://testjobingestion.pythonanywhere.com/autosourceprovision77`
- **RSS Feed**: `https://feeds.bbci.co.uk/news/rss.xml`
- **W3Schools Books**: `https://www.w3schools.com/xml/books.xml`

## CORS Considerations

Since this version runs entirely in the browser, it uses CORS proxy services (allorigins.win, corsproxy.io, codetabs.com) to fetch XML feeds that don't allow direct cross-origin requests. This works for most public XML feeds.

**For password-protected feeds**: Browser security restrictions may prevent authentication through CORS proxies. For those feeds, use the [Flask backend version](https://github.com/akasingh_LinkedIn/xpath-extractor-python) instead.

## Updating the Application

To get the latest updates:

```bash
# Navigate to the project directory
cd ~/Documents/xml-xpath-extractor

# Pull the latest changes
git pull origin main
```

Then refresh your browser to see the updates.

## Files in This Project

- **`index.html`** - Complete standalone application (all HTML, CSS, and JavaScript in one file)
- **`LI-Logo.png`** - LinkedIn logo for the header
- **`README.md`** - This file with instructions

## Differences from Flask Backend Version

| Feature | GitHub Pages Version | Flask Backend Version |
|---------|---------------------|----------------------|
| Installation | ❌ None required | ✅ Python + dependencies |
| Backend Server | ❌ No server needed | ✅ Flask server required |
| CORS Handling | ✅ Uses proxy services | ✅ Server-side fetch |
| Authentication | ⚠️ Limited by browser | ✅ Full support |
| Hosting | ✅ Free on GitHub Pages | ✅ Requires server |
| Offline Use | ✅ Works offline (after loading) | ❌ Needs server running |

## When to Use Which Version?

- **Use GitHub Pages Version** if:
  - You want zero installation
  - Working with public XML feeds
  - Need quick access without setup
  - Want to share with others via URL

- **Use [Flask Backend Version](https://github.com/akasingh_LinkedIn/xpath-extractor-python)** if:
  - Working with password-protected feeds
  - Need guaranteed CORS support
  - Want full control over the server
  - Have complex authentication requirements

## Troubleshooting

### Cannot Fetch XML Feed

If you see CORS errors:
1. Try a different XML feed to verify the app works
2. Check if the feed URL is publicly accessible
3. For authenticated feeds, consider using the [Flask backend version](https://github.com/akasingh_LinkedIn/xpath-extractor-python)

### Page Not Loading Locally

If the page doesn't load:
1. Make sure you're using a local server (Python http.server recommended)
2. Check that you're accessing `http://localhost:8080` (or your port number)
3. Try opening the `index.html` file directly in your browser

### XPaths Not Showing

If XPaths don't appear after clicking "Extract XPaths":
1. Open browser Developer Tools (F12) and check the Console for errors
2. Verify the XML feed URL is correct and accessible
3. Check your internet connection

## Hosting on GitHub Pages (For Advanced Users)

To host your own version:

1. Fork this repository on GitHub
2. Go to repository Settings → Pages
3. Select "main" branch as the source
4. Your site will be available at: `https://YOUR-USERNAME.github.io/xml-xpath-extractor/`

## Need Help?

- Check the [Issues](https://github.com/akasingh_LinkedIn/xml-xpath-extractor/issues) page
- Try the [Flask backend version](https://github.com/akasingh_LinkedIn/xpath-extractor-python) for more complex needs
- Contact the support team

## Author

Designed by [Akash Singh](https://www.linkedin.com/in/akashsinghjsr/)

## Technologies Used

- **HTML5** - Structure
- **CSS3** - Styling with LinkedIn branding
- **Vanilla JavaScript** - All functionality (no frameworks!)
- **CORS Proxies** - Cross-origin request handling
- **DOMParser API** - XML parsing

## License

© 2026 XML XPath Extractor
