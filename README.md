# Nourish

A simple daily meal-plan app for a fatty-liver, weight-loss protocol. Open it on a phone and use **Share → Add to Home Screen** to install it like an app.

- **Today**: what to eat next, exact portions in grams, check-offs, macro and water progress
- **Week**: the Sunday–Saturday plan, a shopping list sized to the real portions, and prep steps
- **Progress**: weekly weigh-ins and a forecast toward the goal weight
- **Me**: daily numbers (carbs are calculated automatically), schedule, body stats, and label values for her daily staples

Everything runs in the browser and data stays on the phone (localStorage). There is no server.

## How the planner works
Each meal is a recipe with flexible parts (protein, carbs, cooking fat) and fixed parts. For each day, a small solver resizes the flexible parts so the day hits her protein, carb, and fat targets. It also keeps each meal's shape: a low-carb breakfast with at least 30 g protein and 10 g fat, carbs at lunch and in the afternoon, and dinner by 6:30. Portions are then rounded to kitchen-friendly amounts (5 g, whole eggs, ½ tsp). Swapping a meal or changing the numbers re-balances the day.

Nutrition values come from USDA FoodData Central. Meat and fish weights are cooked weight.
