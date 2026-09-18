# AgroPulse

Agricultural intelligence platform providing crop management, market data, and farming advisory services.

Built at Sreenithi Hackathon.

## Overview

AgroPulse is a full-stack TypeScript application that gives farmers and agricultural stakeholders access to crop management tools, market price data, and AI-assisted farming guidance through a unified web interface.

## Features

- Crop management and tracking dashboard
- Market price monitoring
- Agricultural advisory system
- Monorepo structure with shared types between client and server
- Docker containerized deployment

## Tech Stack

| Component | Technology |
|-----------|------------|
| Frontend | React, Vite, Tailwind CSS |
| Backend | Node.js, Express, TypeScript |
| ORM | Drizzle ORM |
| Containerization | Docker |
| Build tool | Vite |
| Type sharing | Shared `/shared` package |

## Project Structure

```
├── client/         # React frontend
├── server/         # Node.js + Express backend
├── shared/         # Shared TypeScript types
├── script/         # Utility scripts
├── AgroPulse-HF/   # Hugging Face deployment configuration
├── Dockerfile
├── drizzle.config.ts
└── vite.config.ts
```

## Running Locally

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

## Deployment

Containerized with Docker and configured for Hugging Face Spaces deployment.

```bash
docker build -t agropulse .
docker run -p 3000:3000 agropulse
```

## Future Improvements

- Add real-time market price feeds
- Integrate weather API for farming advisories
- Add crop disease detection using image recognition
- Expand regional crop database

## Author

**S. Kavin Raj**
[LinkedIn](https://www.linkedin.com/in/s-kavin-raj/) · [GitHub](https://github.com/S-Kavin-Raj/)
