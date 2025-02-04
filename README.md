Below is a **concise, updated README** incorporating the **code structure** you provided. You can adjust sections as needed to match your specific setup or preferences.

---

# Bolatejao

Bolatejao is a modern, interactive web application designed to engage users in localized news discussions. It’s built with **Next.js (App Router)**, **TypeScript**, **Tailwind CSS**, and **Framer Motion**, supporting real-time community engagement and audio-based commenting.

## Table of Contents

1. [Features](#features)  
2. [Technology Stack](#technology-stack)  
3. [Project Structure](#project-structure)  
4. [Installation](#installation)  
5. [Usage](#usage)  
6. [Contributing](#contributing)  
7. [License](#license)  

---

## Features

- **Trending News Feed**: Categorized news articles with share functionality and infinite scroll.  
- **Discussion Pages**: In-depth comment threads (text and audio) with real-time updates.  
- **User Profiles**: Profile pages with activity stats and reputation score.  
- **Fact-Checking & Moderation**: Integration with the Perspective API to filter inappropriate content and verify facts.  
- **Sentiment Insights**: Analyze community sentiments around specific news topics.

---

## Technology Stack

- **Next.js (App Router)**: Server-side rendered React components and built-in API routes for streamlined development.  
- **TypeScript**: Enforced type safety for cleaner, maintainable code.  
- **Tailwind CSS**: Utility-first framework for responsive styling.  
- **Framer Motion**: Smooth animations and transitions in React.  
- **WebSockets**: Real-time data flow for interactive discussions and updates.

---

## Project Structure

Below is the simplified folder layout following **Next.js 13+ App Router** conventions:

```
/
├─ app/
│   ├─ api/
│   │   ├─ comments/
│   │   │   └─ route.ts
│   │   └─ news/
│   │       └─ route.ts
│   ├─ components/
│   │   ├─ CommentForm.tsx
│   │   ├─ CommentItem.tsx
│   │   ├─ CommentList.tsx
│   │   ├─ DiscussionThread.tsx
│   │   ├─ FactCheckCard.tsx
│   │   ├─ Footer.tsx
│   │   ├─ InfiniteScroll.tsx
│   │   ├─ LatestUpdate.tsx
│   │   ├─ LoadingAnimation.tsx
│   │   ├─ Navbar.tsx
│   │   ├─ NewsCard.tsx
│   │   ├─ NewsItem.tsx
│   │   ├─ SentimentInsightsCard.tsx
│   │   ├─ TrendingNewsFeed.tsx
│   │   ├─ TrendingTopics.tsx
│   │   ├─ TrendingTopicSummary.tsx
│   │   ├─ UserReputation.tsx
│   │   └─ UserStats.tsx
│   ├─ discussion/
│   │   └─ [id]/
│   │       └─ page.tsx
│   ├─ profile/
│   │   └─ page.tsx
│   ├─ globals.css
│   ├─ layout.tsx
│   └─ page.tsx
├─ public/
└─ package.json
```

### Key Files

- **`app/layout.tsx`**: The root layout that wraps all pages.  
- **`app/page.tsx`**: The home page component.  
- **`app/globals.css`**: Global Tailwind CSS styles.  
- **`app/discussion/[id]/page.tsx`**: Dynamic route for individual discussion pages.  
- **`app/profile/page.tsx`**: User profile page.  
- **`app/api/comments/route.ts`**: Handles comment-related API requests.  
- **`app/api/news/route.ts`**: Handles news-related API requests.

This structure supports easy scaling and maintenance, with a clear separation of concerns between routes, components, and API logic.

---

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/bolatejao.git
   cd bolatejao
   ```
2. **Install dependencies**:
   ```bash
   npm install
   ```
   or
   ```bash
   yarn
   ```
3. **Set up environment variables** (if needed):
   - Create a `.env.local` file at the root with any necessary environment variables (e.g., API keys).

---

## Usage

1. **Development server**:
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) to view in your browser.

2. **Production build**:
   ```bash
   npm run build
   npm run start
   ```
   This creates an optimized production build of your Next.js application.

3. **Deployment**:
   - **Vercel**: Connect your GitHub repo to Vercel. It automatically builds and deploys on each push to the main branch.  
   - **Other hosts**: You can deploy any Next.js build output on platforms that support Node.js.

---

## Contributing

1. **Fork** the repository (if you’re external to the project).  
2. **Create a feature branch**:
   ```bash
   git checkout -b feature/some-improvement
   ```
3. **Commit your changes** with clear messages:
   ```bash
   git commit -m "Add new discussion feature"
   ```
4. **Push** to your branch:
   ```bash
   git push origin feature/some-improvement
   ```
5. **Create a Pull Request** to the `main` branch on GitHub.  

For major changes or suggestions, please open an **issue** to discuss them first.

---

## License

*(Optional) Choose a suitable license (e.g., [MIT](https://opensource.org/licenses/MIT)) if you intend to open-source the project, or specify that the code is proprietary if not.*

---

**Enjoy collaborating on Bolatejao!**  
Feel free to open issues or discussions for feedback, questions, or contributions.
