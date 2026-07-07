# Nutrient Optimization: Recipe Tracker

CodePath WEB103 Final Project

Designed and developed by:
- Damaris Campos
- Amanda Gray
- Sergio Montufar
- Nathachanok Netmaneesuk
- Beatrice Olaosebikan
- Danielle Phillips

🔗 Link to deployed app:

## About

### Description and Purpose

Nutrient Optimization: Recipe Tracker is a social media application for sharing and discovering home-cooked meals. It allows users to log their recipes, track the micro and macronutrients automatically—derived from a database of the most common ingredients for each food group with standard serving sizes—and interact with a community of food lovers by liking, saving, and commenting on posts.

### Inspiration

The inspiration is a mix of a social media platform and a food tracking app. The concept behind Nutrient Optimization: Recipe Tracker was to give people a dedicated space to catalog exactly what goes into their meals. This app will enable users to create delicious meals while staying informed about their nutritional value. The goal for the app is to provide an easy way to organize recipes, track ingredients, and share dishes with others.

## Tech Stack
Frontend: React, JavaScipt, React Router

Backend: TypeScript, Node.js, CORS, Express, Postgres Database, Render

## Features

### Required
***

### Login/Sign Up Page:
A page for users to log in and sign up securely, enabling them to modify their own posts.

[gif goes here]

### Recipe Feed

The home page displays a feed of all community-shared recipes pulling from the database. It serves as the primary read function where users can browse existing posts.

[gif goes here]

### Detailed Recipe View

Clicking on a recipe utilizes React Router dynamic routing to redirect the user to a dedicated details page. This page displays the full breakdown of ingredients, step-by-step preparation instructions, the calories, protein, fats, and other micronutrients, and the author profile link.

[gif goes here]

### Interactive Recipe Creation

Users can publish new content via a recipe creation form. They can input the recipe title, instructions, upload an image link, and select ingredients from each food group. There will be a dropdown menu for each food group: Grains, Protein, Vegetables, Fruits, Fats & Oils, and Other (seasonings). The options would be the most common ingredients in the world falling into the food group selected and would include a standard serving size. There would be an input box where users can input the ratio of the serving size (if the serving size is 1/4 cup of uncooked basmati rice, but the user used 1 cup, they would input 4 for the ratio).
[gif goes here]

### Recipe Management

Users can modify their existing recipes or remove their posts from the application. They can only modify and delete their own posts and no one else's. This section also includes the administrative function to reset the database to its default state, fulfilling the baseline RESTful API and database requirements.


[gif goes here]

### Custom Features

### Nutritional Value Filtering and Sorting

Fulfills the custom features requirement for filtering and sorting. The main feed includes a custom filtering system allowing users to sort or filter recipes by the nutrient value of an ingredient, such as high healthy fats, high protein (30 or more grams), low (500 or less) or high calorie (800+), and more.

[gif goes here]

### Custom Recipe Cards

Fulfills the custom feature requirement for a one-to-one database relationship by linking the core Recipe table directly to a separate RecipeCard table which contains the dish image and title. This allows users to customize how their dish appears in the main feed by storing visual settings separately from the ingredient and instruction text.

### User Validation when modifying post
Fulfills the custom feature requirement that data submitted via a POST or PATCH request is validated before the database is updated. Before a user can modify a post, we use the foreign key database relationship to verify that the user id for the post matches the user id of the current user.

### Macro and Micronutrients Calculations .
Fulfills the custom feature requirement that data is automatically generated in response to a certain event or user action. When a user inputs ingredients and their respective serving size ratio, nutrients are automatically calculated.

[gif goes here]


### [ADDITIONAL FEATURES GO HERE - ADD ALL FEATURES HERE IN THE FORMAT ABOVE; you will check these off and add gifs as you complete them]

### Cannot Modify Alert:
Fulfills the stretch feature. Toast messages deliver simple feedback in response to user events. If a user tries to click the edit button of a post that is not their own, a toast message appears saying they can't modify a post that does not belong to them.

[gif goes here]

### One to Many Databse:
The recipe database would have a one-to-many relationship with the food group database, where the ingredient ID in the food group database would be a foreign key in the recipe database.

[gif goes here]



## Installation Instructions

[instructions go here]
