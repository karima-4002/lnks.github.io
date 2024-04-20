<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script >
   // Get all the tiles on the front page
const tiles = document.querySelectorAll('.tile');

// Get the Specials tile
const specialsTile = tiles[1];

// Add a click event listener to the Specials tile
specialsTile.addEventListener('click', () => {
  // Get an array of all the menu categories
  const categories = ['Lunch', 'Dinner', 'Sushi', 'Desserts'];

  // Generate a random index for a category
  const randomIndex = Math.floor(Math.random() * categories.length);

  // Get the random category
  const randomCategory = categories[randomIndex];

  // Redirect the user to the single category page for the selected menu category
  window.location.href = `/category/${randomCategory}`;
});
    </script>
</body>
</html>
