# Bash-Workout
A small tool to help you run through your workout routine via bash.

## Installation
```bash
wget https://raw.githubusercontent.com/cogwizzle/bash-workout/bash-workout -O /usr/local/bin/bash-workout
```

## Usage
Create a csv file with your workout routine. The first column is the workout. The second column is the time in seconds.
```csv
sit throughs,30
push ups,30
sit ups,45
body squats,45
russian twists,45
burpees,30
pike push ups,30
heel taps,45
```

Run the tool with the CSV file as input.
```bash
cat workout.csv | bash-workout
```

You can adjust the break duration by setting the `BREAK_DURATION`.
```bash
export BREAK_DURATION=30 ; cat workout.csv | bash-workout
```

You can adjust the text to speach command by setting the `SPEACH_COMMAND`.
```bash
export SPEACH_COMMAND="say" ; cat workout.csv | bash-workout
```
