<-- HTML-->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Layout</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <!-- Navigation Bar -->
  <nav class="navbar">
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <!-- Main Content -->
  <div class="content">
    <section class="section section-left">Section 1</section>
    <section class="section section-right">Section 2</section>
  </div>
</body>
</html>
<--CSS-->
/* General Styles */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

.navbar {
  background-color: #333;
  padding: 10px 0;
}

.navbar ul {
  display: flex;
  justify-content: center;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.navbar li {
  margin: 0 15px;
}

.navbar a {
  color: white;
  text-decoration: none;
  font-size: 18px;
}

.content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
  padding: 20px;
}

.section {
  background-color: #f4f4f4;
  padding: 20px;
  border-radius: 8px;
}

/* Media Queries */
@media (max-width: 768px) {
  .content {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 480px) {
  .navbar ul {
    flex-direction: column;
    align-items: center;
  }
  
  .navbar li {
    margin: 10px 0;
  }
}

