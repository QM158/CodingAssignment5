<body>
  <div class="page-grid">
    <header class="main-header">
      <h1>🌅 Welcome to Our Recipe Hub</h1>
    </header>

    <section class="content-row second-row">
      <div class="column links">
        <h2>🔗 Links</h2>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Recipes</a></li>
          <li><a href="#">Tips</a></li>
        </ul>
      </div>
      <div class="column content">
        <h2>🍝 Featured Recipe</h2>
        <img src="https://via.placeholder.com/300x200.png?text=Dish" alt="Dish image">
        <p>A delightful dish made with fresh ingredients and love.</p>
      </div>
      <div class="column rating">
        <h2>⭐ Ratings</h2>
        <p>🌟🌟🌟🌟☆</p>
        <button>Convert Units</button>
      </div>
    </section>

    <section class="content-row third-row">
      <div class="column ingredients">
        <h2>🥕 Ingredients</h2>
        <ul>
          <li>1 cup flour</li>
          <li>2 eggs</li>
          <li>½ cup milk</li>
        </ul>
      </div>
      <div class="column equipment">
        <h2>🧰 Equipment</h2>
        <ul>
          <li>Mixing bowl</li>
          <li>Whisk</li>
          <li>Pan</li>
        </ul>
      </div>
      <div class="column directions">
        <h2>📋 Directions</h2>
        <ol>
          <li>Mix ingredients.</li>
          <li>Heat pan.</li>
          <li>Cook and serve.</li>
        </ol>
      </div>
    </section>

    <footer class="main-footer">
      <p>© 2025 Recipe Hub. Crafted with 🍂 by Mr.</p>
    </footer>
  </div>
  /* 🧱 Page-wide grid container */
.page-grid {
  display: grid;
  grid-template-rows: auto 1fr 1fr auto;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 2rem;
}

/* 🧭 Header and Footer spanning full width */
.main-header, .main-footer {
  grid-column: 1 / -1;
  text-align: center;
  background-color: #ffe0b2;
  padding: 1.5rem;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

/* 🧩 Each content row uses grid layout */
.content-row {
  display: contents; /* allow child columns to fill the parent grid */
}

/* 💡 Columns inside each row */
.column {
  background: linear-gradient(to bottom, #fff3e0, #ffe0b2);
  border: 2px solid #d2691e;
  border-radius: 16px;
  padding: 1rem;
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.15);
  text-align: center;
}

/* 🎯 Links styling */
.links a {
  text-decoration: none;
  color: #b2541c;
  font-weight: bold;
}

.links a:hover {
  color: #6b4c2f;
}

/* 📱 Mobile-friendly layout */
@media screen and (max-width: 768px) {
  .page-grid {
    grid-template-columns: 1fr;
    grid-template-rows: repeat(4, auto);
  }

  .main-header, .main-footer {
    grid-column: 1;
  }

  .column {
    margin-bottom: 1rem;
  }
}

</body>
