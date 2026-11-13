# GitHub Finder

A frontend React app that searches GitHub users and shows their profile and repositories, using the GitHub API.

**Live demo:** https://github-finder-three-livid.vercel.app/

> Based on a tutorial project.

## Features

- Search GitHub users by username
- User profile page with [avatar, login]
- List of the user's public repositories
- [Loading state while data is fetched]

## Built with

- React
- [Vite]
- [React Router]
- [Tailwind CSS / CSS]
- [Context API]
- GitHub REST API

## Run locally

```bash
git clone https://github.com/denis-rafajlovski/github-finder.git
cd github-finder
npm install
npm run dev
```

If the project needs environment variables, create a `.env.local` file:

```
VITE_GITHUB_URL=https://api.github.com
```

## Known limitations

- The GitHub API allows a limited number of unauthenticated requests per hour, so heavy use can hit the rate limit.
- This is a frontend-only app. Any token placed in a `VITE_` variable ends up in the browser bundle, so I don't use a personal token here. In production I would call the API through a small backend.
