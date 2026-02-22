# ResearchHub
Search, scrape, and analyze any website. used Firecrawl. ® Extract structured content, discover sitemaps, and research the web with a professional-grade toolkit built on the Firecrawl API.


| ![](images/showcase/id-preview--ff350870-5ccb-402b-b8b7-a46fe655add3.lovable.app.png) |
|:--:|
|  | 

| ![](images/showcase/id-preview--ff350870-5ccb-402b-b8b7-a46fe655add3.lovable.app%20(5).png) |
|:--:|
|  | 



| ![](images/showcase/id-preview--ff350870-5ccb-402b-b8b7-a46fe655add3.lovable.app%20(4).png) |
|:--:|
|  | 







| ![](images/showcase/id-preview--ff350870-5ccb-402b-b8b7-a46fe655add3.lovable.app%20(3).png) |
|:--:|
|  | 


A professional-grade web research toolkit that lets you search, scrape, and map any website directly from your browser. Built with React, TypeScript, and powered by the [Firecrawl](https://www.firecrawl.dev) API.

![Content Research Hub](https://i.ibb.co.com/bR5TMSSM/rsearchcropped.png)



## Table of Contents

- [About](#about)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Getting Your Firecrawl API Key](#getting-your-firecrawl-api-key)
- [Usage Guide](#usage-guide)
- [Contributing](#contributing)
- [License](#license)



## About

Content Research Hub is a client-side web application designed for researchers, developers, content creators, and anyone who needs to extract meaningful data from websites. It connects directly to the Firecrawl API using your own API key, which is stored securely in your browser's local storage and never sent to any third-party server.

No backend server is required. Everything runs in your browser.



## Features

### Web Search

- Search the entire web using natural language queries.
- Get back a list of results with titles, URLs, and descriptions.
- Optionally toggle "Include content" to pull the full markdown content from each search result.
- Results are displayed in a clean, readable card layout.

### Website Scraping

- Enter any URL and extract its content in multiple formats at the same time.
- Supported output formats:
  - **Markdown** , Clean, readable text content of the page. Perfect for saving articles or feeding into other tools.
  - **HTML** , The processed HTML with scripts and styles stripped out.
  - **Links** , A complete list of every URL found on the page.
  - **Summary** , An AI-generated concise summary of the page content.
  - **Screenshot** , A full-page screenshot rendered as an image.
- Toggle any combination of formats before scraping.
- One-click copy button for markdown content.
- Metadata display showing page title, description, language, and HTTP status code.

### Website Mapping

- Discover all the pages and URLs that belong to a website.
- Enter a root URL and the tool will return up to 200 discovered URLs.
- Use the optional keyword filter to narrow results down to specific sections or topics.
- Each URL is clickable and opens in a new tab.
- Great for understanding the structure of a website before doing deeper research.

### API Key Management

- Simple, secure setup screen where you paste your Firecrawl API key.
- The key is validated against the Firecrawl API before being accepted.
- Your key is stored only in your browser's localStorage. It never leaves your machine.
- Disconnect at any time with one click, which removes the key from storage entirely.

### User Interface

- Dark-themed, terminal-inspired design with clean typography.
- Fully responsive layout that works on desktop, tablet, and mobile.
- Smooth animations on page load.
- Tabbed dashboard interface for switching between Search, Scrape, and Map tools.
- Clear error messages and loading states for every action.






## Prerequisites

Before you start, make sure you have these installed on your machine:

- **Node.js** version 18 or higher , [Download here](https://nodejs.org)
- **npm** (comes bundled with Node.js) or **bun** as your package manager
- **Git** , [Download here](https://git-scm.com)
- A **Firecrawl API key** (free tier available) , [Get one here](https://www.firecrawl.dev)

To check if you already have Node.js and npm installed, open your terminal and run:

```bash
node --version
npm --version
```

You should see version numbers printed. If not, install Node.js first.



## Installation

Follow these steps to get the project running on your local machine.

**Step 1: Clone the repository**

```bash
git clone https://github.com/odaysec/ResearchHub.git
```

**Step 2: Navigate into the project folder**

```bash
cd ResearchHub
```

**Step 3: Install dependencies**

Using npm:

```bash
npm install
```

Or if you prefer bun:

```bash
bun install
```

This will download and install all the required packages listed in package.json. It may take a minute or two depending on your internet connection.

**Step 4: Start the development server**

Using npm:

```bash
npm run dev
```

Or with bun:

```bash
bun run dev
```

**Step 5: Open in your browser**

Once the server starts, you will see a message like this in your terminal:

```
VITE v5.x.x  ready in 300ms

Local:   http://localhost:5173/
```

Open that URL in your browser. You should see the Content Research Hub landing page.



## Getting Your Firecrawl API Key

1. Go to [firecrawl.dev](https://www.firecrawl.dev) and create a free account.
2. Once logged in, navigate to your dashboard.
3. Find the API Keys section and generate a new key.
4. Copy the key. It will look something like `fc-xxxxxxxxxxxxxxxxxxxxxxxx`.
5. Paste it into the API key setup screen in the app.

The free tier gives you a generous number of API calls to get started. You can upgrade later if you need more.



## Usage Guide

### Connecting Your API Key

When you first open the app, you will see the "Connect Firecrawl" screen. Paste your API key into the input field and click "Connect." The app will verify your key by making a test request. If the key is valid, you will be taken to the Research Dashboard.

### Using the Search Tab

1. Click on the "Search" tab in the dashboard.
2. Type your search query in the input field. For example: "best practices for web accessibility."
3. If you want the full page content included with each result, check the "Include content" checkbox.
4. Click the "Search" button.
5. Results will appear as cards showing the title, URL, and description. If you enabled "Include content," you can expand each result to see the full markdown content.

### Using the Scrape Tab

1. Click on the "Scrape" tab.
2. Enter the full URL of the page you want to scrape. For example: `https://example.com`.
3. Select which formats you want by clicking the format buttons (Markdown, HTML, Links, Summary, Screenshot). You can select multiple.
4. Click the "Scrape" button.
5. The results will appear in organized sections. You can copy markdown content with one click, view the screenshot, browse extracted links, or read the AI-generated summary.

### Using the Map Tab

1. Click on the "Map" tab.
2. Enter the root URL of the website you want to map. For example: `https://docs.example.com`.
3. Optionally, type a keyword in the filter field to narrow down the discovered URLs.
4. Click the "Map" button.
5. A numbered list of all discovered URLs will appear. Each one is clickable and opens in a new tab.

### Disconnecting
Click the "Disconnect" button in the top-right corner of the dashboard. This removes your API key from the browser and takes you back to the setup screen.





## Contributing

Contributions are welcome. If you would like to improve this project:

1. Fork the repository.
2. Create a new branch for your feature or fix: `git checkout -b my-feature`.
3. Make your changes.
4. Test everything locally to make sure it works.
5. Commit your changes: `git commit -m "Add my feature"`.
6. Push to your branch: `git push origin my-feature`.
7. Open a Pull Request on GitHub.

Please keep your code clean, follow the existing code style, and write meaningful commit messages.



## License

This project is open source. Built by [odaysec](https://github.com/odaysec).



## Credits

- [Firecrawl](https://www.firecrawl.dev) for the web scraping and search API
- [shadcn/ui](https://ui.shadcn.com) for the beautifully designed UI components
- [Vite](https://vitejs.dev) for the blazing fast development experience


<p align="center">
  <a href="https://star-history.com/#odaysec/ResearchHub&Date">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=odaysec/ResearchHub&type=Date&theme=dark" />
     <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=odaysec/ResearchHub&type=Date" />
     <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=odaysec/ResearchHub&type=Date" />
   </picture>
  </a>
