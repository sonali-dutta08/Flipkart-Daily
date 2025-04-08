This is a simple in-memory inventory management system designed for a Flipkart Daily-like application. It enables users to add grocery items, manage stock, and search inventory using multiple filters and sorting options by Sonali.

## ✅ Features

- **Add Items** to the catalog with category, brand, and price.
- **Add Inventory** by increasing quantity of existing items.
- **Search Inventory** using:
  - Filter by Category
  - Filter by Brand
  - Filter by Price Range
  - Combination of filters (e.g., category + brand, category + price)
- **Sorting Search Results** by:
  - Price (Ascending / Descending)
  - Quantity (Ascending / Descending)
- Designed with extensibility and modularity in mind.
- No database used — data stored using Java collections (in-memory).

addItem("Amul", "Milk", 100);
addItem("Nestle", "Milk", 60);
addInventory("Amul", "Milk", 10);
addInventory("Nestle", "Milk", 5);

searchItemsByBrand("Nestle"); // Output: Nestle Milk 5
searchItemsByCategory("Milk"); // Output: Amul Milk 10, Nestle Milk 5
searchItemsByPriceRange(50, 90); // Output: Nestle Milk 5
