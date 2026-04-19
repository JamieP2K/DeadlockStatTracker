# DeadlockStatTracker

A web application built with ASP.NET Core for tracking player statistics, match history, and hero performance in Valve's **Deadlock**.

---

## Description

DeadlockStatTracker lets you look up any Deadlock player and view a breakdown of their performance — including recent match history, overall stats, and per-hero metrics. It pulls live data from the [deadlock-api.com](https://deadlock-api.com) community API and presents it in a clean, readable web interface.

Built as a portfolio project to demonstrate ASP.NET Core development, RESTful API integration, and frontend data presentation.

---

## Features

- **Match History** — Browse a player's recent matches with outcomes, duration, KDA, and hero played
- **Player Stats** — Overall win rate, average KDA, most-played heroes, and performance trends
- **Hero / Character Stats** — Per-hero breakdown including wins, losses, average damage, and more

---

## Tech Stack

| Layer | Technology |
|---|---|
| Language | C# (.NET 8+) |
| Framework | ASP.NET Core |
| Data Source | [deadlock-api.com](https://deadlock-api.com) |

---

## Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download) or later
- A valid API key from [deadlock-api.com](https://deadlock-api.com) (if required by the endpoint)
- Git

---

## How to Use

1. **Search for a player** — Enter a Steam ID or player name in the search bar on the homepage
2. **View match history** — Click a player to see their recent matches, including hero, outcome, KDA, and duration
3. **Explore player stats** — Navigate to the stats tab for aggregated performance data and win rates
4. **Browse hero stats** — Select a specific hero to see the player's performance broken down by character

---

## Project Structure

```
DeadlockStatTracker/
├── Controllers/        # ASP.NET MVC controllers
├── Models/             # Data models and API response DTOs
├── Services/           # HTTP client wrappers for deadlock-api.com
├── Views/              # Razor views
├── wwwroot/            # Static assets (CSS, JS)
├── appsettings.json    # App configuration (API keys, etc.)
└── Program.cs          # App entry point
```

> Structure will be updated as the project develops.

---

## Todo / Roadmap

### Setup
- [ ] Initialize ASP.NET Core project
- [ ] Configure `IHttpClientFactory` for deadlock-api.com
- [ ] Set up appsettings.json for API key management

### Core Features
- [ ] Player search by Steam ID or username
- [ ] Match history page
- [ ] Individual player stats page
- [ ] Hero / character stats breakdown

### Polish
- [ ] Responsive UI and styling
- [ ] Error handling and loading states
- [ ] Response caching to reduce API calls

### Deployment
- [ ] Deploy to Azure / Railway / Fly.io

---

## API Reference

This project uses the **deadlock-api.com** community API.

- Base URL: `https://api.deadlock-api.com`
- Documentation: [deadlock-api.com/docs](https://deadlock-api.com/docs)

> Note: deadlock-api.com is a third-party community API and is not affiliated with Valve.

---

## License

This project is licensed under the [MIT License](LICENSE).