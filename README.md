# brisbane-bullets-player-load-analysis
End-to-end sports analytics project using Excel, Power Query and Power BI to analyse player workloads, identify load spikes (>20%), monitor athlete risk and generate coach-focused performance insights.

Project Overview

This project was completed as part of a sports science internship assessment based on player tracking data collected across a basketball season.

The objective was to analyse player workload data and answer three practical coaching questions:

Which player accumulated the highest load throughout the season?
Were there any workload spikes (>20% increase week-to-week) for the team or individual players?
What additional performance insights can be learned from the dataset?

The project demonstrates a complete sports analytics workflow involving:

Data cleaning in Excel
Data transformation in Power Query
Data modelling and DAX calculations in Power BI
Coach-focused reporting and storytelling
Dataset Overview

The dataset contained session-based player tracking metrics for 9 players across 16 training sessions.

Key Metrics Included
Metric	Description
Accumulated Acceleration Load	Total workload accumulated during session
Acceleration Load (THIL)	High intensity acceleration workload
Accelerations	Number of acceleration efforts
Decels Load	Deceleration workload
Distance (mi)	Total distance covered
Duration Minutes	Session duration
Sprints	Sprint count
Sprints / min	Sprint density
Speed (% Max)	Relative intensity
Speed Max	Peak speed
FCTs	Change of direction actions
FCTs High	High intensity directional changes
Mechanical Intensity	Overall movement intensity
Jump Height Max	Maximum jump performance

Data Cleaning Process

Step 1 – Excel Cleaning

The raw data was not immediately analysis-ready.Before Cleaning- Data set contained 685 Records

Each session contained:

Player rows
"Ø All Players" summary rows
Repeated headers
Empty rows

Cleaning Steps

Created SessionID

Because sessions did not have unique identifiers, a SessionID column was created.

This allowed session-based calculations later in Power BI.

Removed Unwanted Rows

Only actual player observations were retained.

Converted Time to Minutes
This enabled numerical analysis.

Step 2 – Power Query Cleaning

After importing into Power BI:

Tasks Completed
Verified data types
Converted numeric fields
Checked null values
Rounded metrics where required
Removed remaining invalid rows



Final dataset:

450 records
16 sessions
9 players
18 performance metrics

The dataset was now ready for analysis.

Question 1
Which Player Had The Highest Load Throughout The Season?

### Result

🏀 Player 2 accumulated the highest load throughout the season.

Total Load ≈ 24.4K
Coaching Insight

Player 2 experienced the greatest workload exposure and should be closely monitored for fatigue and recovery management.

Question 2
Were There Any Load Spikes (>20%) Week-To-Week?
Team Load Spike Analysis

Coaching Insight

Several substantial workload increases occurred during the season.

The most significant spike occurred in Week 16.

Such increases may elevate fatigue and injury risk if not planned appropriately.

Individual Player Spike Analysis

The same methodology was applied to each player.

Player weekly loads were compared against the player's previous week.

A spike was recorded when:

Load Increase > 20%
Key Findings

Frequent spikes were observed for:

Player 2
Player 6
Player 8

These players demonstrated repeated exposure to large workload increases.

Coaching Insight

These athletes may require:

Additional recovery monitoring
Modified training loads
Fatigue management strategies
Question 3
Is There Anything Else To Be Learned?

To move beyond the assessment requirements, additional exploratory analysis was performed.

Key Influencer Analysis

Target Variable:

Accumulated Acceleration Load

Factors Tested:

Distance
Duration Minutes
Decels Load
Accelerations
Mechanical Intensity
Findings

Power BI Key Influencers identified:

Distance Covered

Strongest influence on workload.

When distance increased:

Accumulated Acceleration Load increased by approximately 111.6 units
Deceleration Load

Second strongest contributor.

Higher braking demands resulted in higher total workload.

Session Duration

Longer sessions naturally accumulated greater loads.

Accelerations

More acceleration actions increased total load exposure.

Coach Insights
Workload Drivers

The strongest contributors to player load were:

Distance Covered
Deceleration Load
Session Duration
Accelerations
Risk Management

Repeated workload spikes were identified across multiple players.

Monitoring these spikes can help:

Reduce overtraining risk
Improve recovery planning
Support return-to-play decisions
Performance Monitoring

Rather than only monitoring total load, coaches should track:

Distance
Deceleration Load
Acceleration Frequency
Session Duration

These metrics provide earlier warning signs of excessive workload accumulation.

This project successfully transformed raw player tracking data into actionable sports science insights.

Key outcomes included:

1. Identifying the highest workload athlete

2. Detecting team and player workload spikes exceeding 20%

3. Discovering workload drivers using Key Influencer analysis

4. Producing coach-friendly dashboards to support training load management and athlete monitoring

The analysis demonstrates how sports analytics can convert wearable tracking data (Catapault) into evidence-based coaching decisions that improve athlete performance while reducing workload-related risk.
