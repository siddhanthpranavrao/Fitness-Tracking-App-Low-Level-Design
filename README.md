# Fitness Tracking App

### Requirements

1. The app should poll data every 15 mins for the day
2. The data sent over to the app contains
   1. Steps
   2. Calories Burnt
   3. Minutes of Workout
   4. Average Heartbeat
   5. Water Intake (ml)
3. The app should give rewards once goals are achieved
   1. The user can set the goals
4. The app should give motivation when
   1. Close to the goal (90%)
   2. Very far away from goal (20%)
   3. Admin configures when to send motivation
5. Types of Goals
   1. Steps Goal
   2. Calorie Goal
   3. Workout Goal
   4. Water Intake Goal
6. Analytics
   1. Weekly and Monthly Graphs
      1. For Steps
      2. For Workout Time
      3. For Calorie
      4. For Water Intake
      5. For number of goals achieved per day
      6. Average Heart Beat

### MAIN Method Flow

1. System sets motivation configuration
2. User sets goals their goals for steps, calories, workout time, water intake
3. Poll for per day data for the user
4. Check the progress of the user
5. Send necessary motivation and give awards for any goal completion
6. Analytics of steps, calories, workout time, water intake, average heart beat (Monthly/ Weekly)

### Classes

1. Person
   1. User
   2. Admin
2. FitnessData
3. Motivation
   1. CloseToGoalMotivation
   2. FarAwayFromGoalMotivation
4. Goal
   1. StepsGoal
   2. CalorieGoal
   3. WorkoutGoal
   4. WaterIntakeGoal
5. GoalStatus (ENUM)
   1. ACHIEVED
   2. NOT_STARTED
   3. NOT_COMPLETED
   4. NOT_TRACKED
   5. IN_PROGRESS
   6. CLOSE_TO_FINISH
   7. CLOSE_TO_START
6. Rewards
   1. DailyStepsReward
   2. DailyCalorieBurntReward
   3. DailyWorkoutGoal
   4. DailyWaterIntakeReward
   5. DailyAllGoalsCompletedReward
7. Analytics
   1. Weekly
      1. StepsAnalytics
      2. CalorieAnalytics
      3. WorkoutAnalytics
      4. WaterIntakeAnalytics
      5. AverageHeartBeatAnalytics
   2. Monthly
      1. StepsAnalytics
      2. CalorieAnalytics
      3. WorkoutAnalytics
      4. WaterIntakeAnalytics
      5. AverageHeartBeatAnalytics
8. Configuration