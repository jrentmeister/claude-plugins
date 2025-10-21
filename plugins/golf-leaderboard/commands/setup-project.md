---
description: Set up a new golf leaderboard project with best practices
---

Initialize a new golf leaderboard application with the following structure:

1. **Create Project Structure**
   - Set up frontend and backend directories
   - Configure build tools (Vite/Webpack)
   - Initialize package.json with dependencies

2. **Database Setup**
   - Create schema for tournaments, players, and scores
   - Set up migrations
   - Add seed data for testing

3. **API Endpoints**
   - GET /tournaments - List all tournaments
   - GET /tournaments/:id/leaderboard - Get current standings
   - POST /scores - Submit a new score
   - PUT /scores/:id - Update a score

4. **Frontend Components**
   - LeaderboardTable - Display rankings
   - ScoreCard - Individual player scores
   - TournamentHeader - Tournament info
   - LiveUpdates - Real-time score changes

5. **Configuration**
   - Environment variables
   - API configuration
   - Database connection settings

Ask the user for:
- Project name
- Preferred frontend framework (React/Vue/Svelte)
- Database choice (PostgreSQL/MySQL/Firebase)
- Deployment target (Vercel/Netlify/AWS)

Then scaffold the complete project structure with all necessary files.
