<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sri Sivarama Engineering Works</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f9;
      color: #2c3e50;
    }
    header {
      background: linear-gradient(135deg, #1a1a1a, #4d4d4d);
      color: white;
      padding: 20px;
      text-align: center;
      animation: gradientShift 8s linear infinite;
    }
    header h1 {
      font-size: 2.8em;
      margin: 0;
      text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
    }
    nav {
      display: flex;
      justify-content: center;
      background-color: #333;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    nav a {
      color: white;
      padding: 18px 35px;
      text-decoration: none;
      transition: all 0.3s ease;
      position: relative;
    }
    nav a:hover {
      background-color: #555;
    }
    nav a::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 50%;
      width: 0;
      height: 2px;
      background: #ff6b6b;
      transition: width 0.3s ease, left 0.3s ease;
    }
    nav a:hover::after {
      width: 100%;
      left: 0;
    }
    .container {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      padding: 20px;
      gap: 20px;
    }
    .card {
      background: white;
      border-radius: 15px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
      width: calc(33% - 20px);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      overflow: hidden;
      position: relative;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.2);
    }
    .card img {
      width: 100%;
      height: 250px;
      object-fit: cover;
    }
    .card-content {
      padding: 20px;
    }
    .card-content h2 {
      font-size: 1.6em;
      color: #2c3e50;
      margin-bottom: 10px;
    }
    .card-content p {
      line-height: 1.7;
      color: #666;
    }
    .tools-section {
      background: linear-gradient(135deg, #f8f9fa, #e9ecef);
      padding: 40px 20px;
    }
    .tool-card {
      background: white;
      border-radius: 12px;
      padding: 30px;
      text-align: center;
      transition: transform 0.3s ease;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }
    .tool-card:hover {
      transform: scale(1.05);
    }
    .tool-card i {
      font-size: 2.5em;
      color: #4a90e2;
      margin-bottom: 15px;
    }
    .profile {
      text-align: center;
      padding: 40px 0;
      background: #2c3e50;
    }
    .profile img {
      width: 180px;
      height: 180px;
      border-radius: 50%;
      border: 5px solid #4a90e2;
      box-shadow: 0 0 15px rgba(0,0,0,0.2);
    }
    .profile h3 {
      color: white;
      font-size: 1.8em;
      margin: 15px 0;
    }
    footer {
      background: #1a1a1a;
      color: #aaa;
      padding: 15px;
      text-align: center;
    }
    @keyframes gradientShift {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    /* New Tools Section Styles */
    .tool-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 25px;
      padding: 20px;
    }
    .tool-box {
      background: white;
      border-radius: 12px;
      padding: 25px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }
    .tool-box:hover {
      transform: translateY(-5px);
    }
    .tool-box h3 {
      color: #4a90e2;
      margin-bottom: 15px;
    }
    .tool-box p {
      color: #555;
      line-height: 1.6;
    }
    .tool-box a {
      display: inline-block;
      margin-top: 15px;
      color: #4a90e2;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }
    .tool-box a:hover {
      color: #2c78b3;
    }
    .estimator-form {
      max-width: 600px;
      margin: 0 auto;
      padding: 20px;
      background: #f8f9fa;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    .estimator-form input,
    .estimator-form select {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border: 1px solid #ddd;
      border-radius: 4px;
    }
    .estimator-form button {
      background: #4a90e2;
      color: white;
      padding: 12px 25px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    .estimator-form button:hover {
      background: #2c78b3;
    }
    .result-box {
      margin-top: 20px;
      padding: 15px;
      background: #e8f4ff;
      border-radius: 5px;
      display: none;
    }
  </style>
</head>
<body>
  <header>
    <h1>Sri sivarama engeering</h1>
  </header>
  <nav>
    <a href="#services"><i class="fas fa-cogs"></i> Services</a>
    <a href="#tools"><i class="fas fa-tools"></i> Tools</a>
    <a href="#profile"><i class="fas fa-user-engineer"></i> Profile</a>
  </nav>

  <div class="container" id="services">
    <div class="card">
      <img src="https://via.placeholder.com/400x250?text=ESP+Technology" alt="ESP">
      <div class="card-content">
        <h2>Electrostatic Precipitator (ESP)</h2>
        <p>Advanced air pollution control systems for industrial emissions</p>
      </div>
    </div>
    <div class="card">
      <img src="https://via.placeholder.com/400x250?text=Boiler+Systems" alt="Boiler">
      <div class="card-content">
        <h2>Boiler Systems</h2>
        <p>High-efficiency steam generation solutions for power plants</p>
      </div>
    </div>
    <div class="card">
      <img src="https://via.placeholder.com/400x250?text=Construction+Engineering" alt="Construction">
      <div class="card-content">
        <h2>Construction Engineering</h2>
        <p>Structural design and project management for large-scale constructions</p>
      </div>
    </div>
  </div>

  <section class="tools-section" id="tools">
    <h2 style="text-align: center; color: #4a90e2; padding: 20px;">Engineering Tools</h2>
    <div class="tool-grid">
      <div class="tool-box">
        <h3><i class="fas fa-calculator"></i> Project Cost Estimator</h3>
        <div class="estimator-form">
          <input type="number" id="area" placeholder="Project Area (sq.ft)">
          <select id="material">
            <option value="50">Standard Materials</option>
            <option value="75">Premium Materials</option>
            <option value="100">Ultra Materials</option>
          </select>
          <input type="number" id="labor" placeholder="Labor Hours">
          <button onclick="calculateCost()">Calculate Cost</button>
          <div class="result-box" id="result">
            Estimated Cost: <span id="costValue"></span>
          </div>
        </div>
      </div>

      <div class="tool-box">
        <h3><i class="fas fa-chart-line"></i> Material Calculator</h3>
        <p>Calculate required materials for your projects</p>
        <select id="materialType">
          <option value="concrete">Concrete (kg)</option>
          <option value="steel">Steel (tons)</option>
          <option value="bricks">Bricks (units)</option>
        </select>
        <input type="number" id="quantity" placeholder="Enter Quantity">
        <button onclick="calculateMaterial()">Calculate</button>
        <p>Total Requirement: <span id="materialResult"></span></p>
      </div>

      <div class="tool-box">
        <h3><i class="fas fa-file-contract"></i> Project Proposal Generator</h3>
        <p>Create professional engineering proposals</p>
        <a href="#"><i class="fas fa-download"></i> Download Template</a>
      </div>
    </div>
  </section>

  <div class="profile" id="profile">
    <img src="https://via.placeholder.com/180?text=Profile+Image" alt="Profile">
    <h3>P. Sudheer</h3>
    <p>Chief Engineering Officer</p>
    <div style="margin: 20px;">
      <a href="#" class="profile-link"><i class="fab fa-linkedin"></i></a>
      <a href="#" class="profile-link"><i class="fas fa-envelope"></i></a>
    </div>
  </div>

  <footer>
    &copy; 2023 Sri Sivarama Engineering Works. All rights reserved.
  </footer>

  <script>
    function calculateCost() {
      const area = parseFloat(document.getElementById('area').value) || 0;
      const material = parseFloat(document.getElementById('material').value) || 0;
      const labor = parseFloat(document.getElementById('labor').value) || 0;
      const cost = (area * material) + (labor * 50);
      document.getElementById('costValue').textContent = `₹${cost.toLocaleString()}`;
      document.getElementById('result').style.display = 'block';
    }

    function calculateMaterial() {
      const type = document.getElementById('materialType').value;
      const qty = parseFloat(document.getElementById('quantity').value) || 0;
      let result = 0;
      switch(type) {
        case 'concrete':
          result = qty * 2400; // kg per cubic meter
          break;
        case 'steel':
          result = qty * 0.15; // tons per 100 sq.ft
          break;
        case 'bricks':
          result = qty * 500; // bricks per cubic meter
          break;
      }
      document.getElementById('materialResult').textContent = result.toLocaleString();
    }
  </script>
</body>
</html>
