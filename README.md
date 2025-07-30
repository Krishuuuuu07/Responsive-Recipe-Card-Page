<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Responsive Recipe Card Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
      background: #f7f7f7;
    }

    h1 {
      text-align: center;
      color: #333;
    }

    .recipe-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      margin-top: 30px;
    }

    .recipe-card {
      background: white;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      padding: 20px;
      transition: transform 0.2s;
    }

    .recipe-card:hover {
      transform: translateY(-5px);
    }

    .recipe-title {
      font-size: 20px;
      margin-bottom: 10px;
      color: #5a2a8a;
    }

    .description {
      font-size: 14px;
      margin-bottom: 10px;
    }

    .ingredients, .steps {
      margin-top: 10px;
    }

    .ingredients ul, .steps ol {
      padding-left: 20px;
    }

    @media (max-width: 600px) {
      body {
        padding: 10px;
      }
    }
  </style>
</head>
<body>
  <h1>My Recipe Card Page</h1>

  <div class="recipe-container">
    <!-- Recipe 1 -->
    <div class="recipe-card">
      <div class="recipe-title">Veggie Sandwich</div>
      <div class="description">A quick and easy sandwich loaded with fresh veggies and cheese.</div>
      <div class="ingredients">
        <strong>Ingredients:</strong>
        <ul>
          <li>2 slices of bread</li>
          <li>1 tbsp butter</li>
          <li>Tomato, cucumber, onion</li>
          <li>Cheese slice</li>
          <li>Salt & pepper</li>
        </ul>
      </div>
      <div class="steps">
        <strong>Preparation:</strong>
        <ol>
          <li>Spread butter on bread.</li>
          <li>Add veggies and cheese.</li>
          <li>Season and close the sandwich.</li>
          <li>Grill or toast if desired.</li>
        </ol>
      </div>
    </div>

    <!-- Recipe 2 -->
    <div class="recipe-card">
      <div class="recipe-title">Masala Oats</div>
      <div class="description">A healthy and spicy Indian-style oats breakfast recipe.</div>
      <div class="ingredients">
        <strong>Ingredients:</strong>
        <ul>
          <li>1/2 cup oats</li>
          <li>1 cup water</li>
          <li>Mixed veggies</li>
          <li>1 tsp oil & spices</li>
        </ul>
      </div>
      <div class="steps">
        <strong>Preparation:</strong>
        <ol>
          <li>Heat oil, sauté veggies.</li>
          <li>Add oats and water.</li>
          <li>Add salt, turmeric, chili.</li>
          <li>Cook until thick and serve hot.</li>
        </ol>
      </div>
    </div>

    <!-- Add more recipes here -->
  </div>
</body>
