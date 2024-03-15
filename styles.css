const recipes = [
    { name: "Grilled Chicken Salad", ingredients: ["chicken", "lettuce", "tomato", "cucumber", "olive oil", "salt", "pepper"] },
    { name: "Vegetable Stir-Fry", ingredients: ["broccoli", "carrots", "bell peppers", "onion", "soy sauce", "garlic", "ginger"] },
    { name: "Quinoa Salad", ingredients: ["quinoa", "cucumber", "tomato", "red onion", "olive oil", "lemon juice", "salt", "pepper"] }
];

function searchRecipes() {
    const searchTerm = document.getElementById("search-input").value.toLowerCase();
    const resultsContainer = document.getElementById("recipe-results");
    resultsContainer.innerHTML = "";

    const matchingRecipes = recipes.filter(recipe =>
        recipe.ingredients.some(ingredient => ingredient.includes(searchTerm))
    );

    if (matchingRecipes.length === 0) {
        resultsContainer.innerHTML = "<p>No recipes found.</p>";
    } else {
        matchingRecipes.forEach(recipe => {
            const recipeElement = document.createElement("div");
            recipeElement.classList.add("recipe");
            recipeElement.innerHTML = `<h3>${recipe.name}</h3><p>Ingredients: ${recipe.ingredients.join(", ")}</p>`;
            resultsContainer.appendChild(recipeElement);
        });
    }
}
