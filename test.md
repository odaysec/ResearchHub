# Content Research Hub  Open Source Web Research Toolkit

**Live Demo:** [ResearchHub.vercel.app](https://ResearchHub.vercel.app)
**Repository:** [github.com/odaysec/ResearchHub](https://github.com/odaysec/ResearchHub)



## What is Content Research Hub?
Content Research Hub is a free, open-source web research toolkit that runs entirely in your browser. It lets you search, scrape, and map any website using the [Firecrawl](https://www.firecrawl.dev) API. No backend needed. No server to maintain. Just deploy to Vercel and start researching.
Built with **React**, **TypeScript**, **Vite**, and **Tailwind CSS**, this project is a great example of how you can build a powerful, fully client-side application and deploy it effortlessly on Vercel.



## Why Vercel?
Vercel makes deploying this project incredibly simple. Since Content Research Hub is a static single-page application with no server-side logic, Vercel handles it perfectly.

Here is what Vercel brings to this project:
- **Zero-config deployment**  Push to GitHub, connect to Vercel, and your app is live in seconds.
- **Global CDN**  Your app loads fast for users anywhere in the world thanks to Vercel's edge network.
- **Automatic preview deployments**  Every pull request gets its own preview URL, making it easy to review changes before merging.
- **Custom domains**  Add your own domain with free SSL certificates, no extra setup required.
- **Vite support out of the box**  Vercel detects Vite projects automatically and configures the build for you.




## Features Web Search
Search the entire web using natural language queries. Results come back with titles, URLs, and descriptions. You can also toggle full content extraction to pull the complete markdown from each result page.

### Website Scraping
Enter any URL and extract its content in multiple formats at the same time: You can select any combination of these formats before scraping. Metadata like page title, description, language, and HTTP status code is also displayed.

### Website Mapping
Discover all the pages that belong to a website. Enter a root URL and the tool returns up to 200 discovered URLs. Use the optional keyword filter to narrow results to specific sections. Every URL is clickable and opens in a new tab.

### Secure API Key Management
Users enter their own Firecrawl API key through a simple setup screen. The key is validated before being stored in the browser's localStorage. It never leaves the user's machine and is never sent to any third-party server. Users can disconnect at any time with a single click.


## Tech Stack

| Technology | Role |
|------------|------|
| [React 18](https://react.dev) | UI framework |
| [TypeScript](https://www.typescriptlang.org) | Type safety |
| [Vite](https://vitejs.dev) | Build tool and dev server |
| [Tailwind CSS](https://tailwindcss.com) | Styling |
| [shadcn/ui](https://ui.shadcn.com) | UI component library |
| [react-markdown](https://github.com/remarkjs/react-markdown) | Markdown rendering |
| [remark-gfm](https://github.com/remarkjs/remark-gfm) | GitHub Flavored Markdown |
| [Firecrawl API](https://www.firecrawl.dev) | Web scraping, search, and mapping |
| [Vercel](https://vercel.com) | Hosting and deployment |



## Deploy to Vercel
You can deploy your own instance in under a minute.
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/odaysec/ResearchHub)

Or deploy manually:

1. Fork the repository on GitHub.
2. Go to [vercel.com](https://vercel.com) and sign in with your GitHub account.
3. Click "Add New Project" and select your forked repository.
4. Vercel will automatically detect it as a Vite project. Leave all settings as default.
5. Click "Deploy" and wait about 30 seconds.
6. Your app is now live with a `.vercel.app` URL.

That is it. No build configuration needed. No environment variables to set.



## Local Development

If you want to run it locally before deploying:

```bash
git clone https://github.com/odaysec/ResearchHub.git
cd ResearchHub
npm install
npm run dev
```

Open `http://localhost:5173` in your browser.



## Getting a Firecrawl API Key

1. Go to [firecrawl.dev](https://www.firecrawl.dev) and create a free account.
2. Navigate to your dashboard and find the API Keys section.
3. Generate a new key. It will look like `fc-xxxxxxxxxxxxxxxxxxxxxxxx`.
4. Paste it into the app when prompted.

The free tier provides enough API calls to get started with real research.



## Screenshots
![id-preview--ff350870-5ccb-402b-b8b7-a46fe655add3.lovable.app (4)|690x431](upload://tGRyOY11sHc7x40uFOEESyqQJ8u.jpeg)
![id-preview--ff350870-5ccb-402b-b8b7-a46fe655add3.lovable.app (3)|690x431](upload://jtsPeR8zHqWBFT2HkWXrzaq2kLQ.jpeg)
![id-preview--ff350870-5ccb-402b-b8b7-a46fe655add3.lovable.app|690x431](upload://3tvYGeMNsvCA9jSHQeiOsJ30Mcx.jpeg)




## License
Open source. Built by [odaysec](https://github.com/odaysec).
**If you found this useful, give it a star on [GitHub](https://github.com/odaysec/ResearchHub) and share it with others who might benefit from it.**
