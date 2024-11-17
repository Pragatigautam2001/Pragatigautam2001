git clone https://github.com/your-pragati/property-management.git
cd property-management
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Property Management</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Welcome to Property Management</h1>
  </header>
  <section id="search">
    <h2>Search Properties</h2>
    <form id="search-form">
      <input type="text" id="location" placeholder="Location">
      <input type="number" id="min-price" placeholder="Min Price">
      <input type="number" id="max-price" placeholder="Max Price">
      <button type="submit">Search</button>
    </form>
  </section>
  <section id="properties">
    <h2>Available Properties</h2>
    <div id="property-list">
      <!-- Dynamic property listings -->
    </div>
  </section>
  <script src="script.js"></script>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.6;
}
header {
  background: #0078d4;
  color: white;
  padding: 1rem;
  text-align: center;
}
#search, #properties {
  padding: 1rem;
}
#property-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
}
.property {
  border: 1px solid #ccc;
  padding: 1rem;
  text-align: center;
}
document.getElementById('search-form').addEventListener('submit', function (e) {
  e.preventDefault();
  alert('Search functionality to be implemented!');
});
