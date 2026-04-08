# NHL Betting Optimizer 🏒

A Spring Boot web application that displays NHL team lineups and helps you find the best betting value!

## Features
- Display tonight's NHL games
- View team lineups for each game
- Calculate value ratios for each player (projected points per dollar)
- Beautiful, responsive web interface

## Getting Started

### Prerequisites
- Java 11 or higher
- Maven 3.6+

### Installation & Running

1. **Clone the repository:**
   ```bash
   git clone https://github.com/evan1schultz-afk/firstproject.git
   cd firstproject
   ```

2. **Run the application:**
   ```bash
   mvn spring-boot:run
   ```

3. **Open in your browser:**
   Navigate to `http://localhost:8080`

## Project Structure

```
src/main/java/com/nhlbets/
├── NhlBetsApplication.java      # Main Spring Boot app
├── controller/
│   └── GameController.java      # Handles HTTP requests
└── model/
    ├── Game.java                # Represents a game
    ├── Player.java              # Represents a player
    └── BettingOdds.java         # Represents betting odds
```

## How It Works

### Player Model
- **Name**: Player's full name
- **Team**: Which team they play for
- **Position**: C (Center), RW (Right Wing), etc.
- **Salary**: DraftKings salary (in DFS context)
- **Projected Points**: Estimated points for the night
- **Value Ratio**: Projected Points ÷ Salary = Best value!

### Game Model
- Contains home and away teams
- Stores lineups for both teams
- Game time information

## Next Steps

1. **Integrate Real APIs**
   - NHL API for actual lineups
   - DraftKings API for real odds
   - DailyFaceoff.com scraping for lineup confirmations

2. **Add Features**
   - Betting recommendations based on value
   - Historical player performance
   - User preferences and favorites
   - Mobile optimization

3. **Improve UI**
   - Player search/filter
   - Sort by value ratio
   - Dark mode
   - Real-time updates

## Learning Goals

This project teaches:
- Spring Boot fundamentals
- MVC (Model-View-Controller) pattern
- Thymeleaf templating
- REST API integration
- Data modeling in Java

## License
MIT

## Author
evann1schultz-afk