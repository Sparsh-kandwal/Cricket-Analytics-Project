# Best 11 of T20 World Cup 2022 - Performance-Based Team Selection

## Project Overview
This project analyzes the performance data of players from the T20 World Cup 2022, sourced from the ESPN website. The goal is to identify the best-performing XI players based on key statistical parameters. The selected team aims to:
- Score at least **180 runs** on average.
- Defend at least **150 runs** on average.

## Data Sources
The data is fetched from ESPN, including:
- **Batting Summary**
- **Bowling Summary**
- **Match Results**
- **Player Information**

## Selection Criteria
Players are categorized into different roles, each with specific performance criteria.

### Openers
| Parameter         | Description                          | Criteria  |
|------------------|----------------------------------|-----------|
| Batting Average  | Average runs scored in an innings | > 30      |
| Strike Rate      | Runs scored per 100 balls         | > 140     |
| Innings Batted   | Total innings played              | > 3       |
| Boundary %       | Percentage of runs in boundaries  | > 50      |
| Batting Position | Order in which batter played      | < 4       |

### Anchors / Middle Order
| Parameter         | Description                          | Criteria  |
|------------------|----------------------------------|-----------|
| Batting Average  | Average runs scored in an innings | > 40      |
| Strike Rate      | Runs scored per 100 balls         | > 125     |
| Innings Batted   | Total innings played              | > 3       |
| Avg. Balls Faced | Average balls faced per innings   | > 20      |
| Batting Position | Order in which batter played      | > 2       |

### Finisher / Lower Order Anchor
| Parameter         | Description                          | Criteria  |
|------------------|----------------------------------|-----------|
| Batting Average  | Average runs scored in an innings | > 25      |
| Strike Rate      | Runs scored per 100 balls         | > 130     |
| Innings Batted   | Total innings played              | > 3       |
| Avg. Balls Faced | Average balls faced per innings   | > 12      |
| Batting Position | Order in which batter played      | > 4       |
| Innings Bowled   | Total innings bowled              | > 1       |

### All-Rounders / Lower Order
| Parameter         | Description                          | Criteria  |
|------------------|----------------------------------|-----------|
| Batting Average  | Average runs scored in an innings | > 15      |
| Strike Rate      | Runs scored per 100 balls         | > 140     |
| Innings Batted   | Total innings played              | > 2       |
| Batting Position | Order in which batter played      | > 4       |
| Innings Bowled   | Total innings bowled              | > 2       |
| Bowling Economy  | Runs conceded per over            | < 7       |
| Bowling Strike Rate | Balls required per wicket      | < 20      |

### Specialist Fast Bowlers
| Parameter         | Description                          | Criteria  |
|------------------|----------------------------------|-----------|
| Innings Bowled   | Total innings bowled              | > 4       |
| Bowling Economy  | Runs conceded per over            | < 7       |
| Bowling Strike Rate | Balls required per wicket      | < 16      |
| Bowling Style    | Type of bowling                   | %Fast%    |
| Bowling Average  | Runs conceded per wicket          | < 20      |
| Dot Ball %       | Percentage of dot balls bowled    | > 40      |

## How It Works
1. **Data Collection**: Scrape relevant data from ESPN.
2. **Filtering Players**: Apply the defined criteria to categorize players.
3. **Best XI Selection**: Choose the top performers for each role.
4. **Performance Validation**: Ensure the team meets the target scoring and defending benchmarks.

## Installation and Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/Sparsh-kandwal/Cricket-Analytics-Project.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Cricket-Analytics-Project
   ```

## Contributing
Feel free to fork this repository, open issues, and submit pull requests to enhance the project.
