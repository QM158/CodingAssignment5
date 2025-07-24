/* 🔧 Universal box-sizing */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* 🌅 Body and Font Styling */
body {
  font-family: "Pacifico", cursive, "Georgia", serif;
  background: linear-gradient(to bottom right, #f9ecd0, #fceabb);
  color: #5e4b32;
  padding: 1rem;
}

/* 🎯 Header and Footer Styling */
.main-header,
.main-footer {
  background-color: #ffe0b2;
  padding: 1.5rem;
  text-align: center;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  margin-bottom: 2rem;
}

.main-header h1 {
  margin: 0;
  font-size: 2.8rem;
  color: #a0522d;
  text-shadow: 1px 1px #e7d2a7;
}

.main-footer p {
  margin: 0;
  font-size: 0.95rem;
  color: #6b4c2f;
}

/* 🧱 Row Structure using Flexbox */
.row {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 1rem;
  margin-bottom: 2rem;
}

/* 🧩 Column Styling */
.column {
  flex: 1 1 30%;
  padding: 1rem;
  background-color: #fff3e0;
  border: 2px solid #d2691e;
  border-radius: 16px;
  text-align: center;
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.15);
}

/* 🌐 Responsive Images */
.column img {
  border-radius: 12px;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.25);
  max-width: 100%;
  height: auto;
}

/* 🔗 Link Styling */
a {
  text-decoration: none;
  color: #b2541c;
  font-weight: bold;
}

a:hover {
  color: #6b4c2f;
}

/* 🧾 Lists */
ul, ol {
  list-style: none;
  padding-left: 0;
  margin-left: 0;
  text-align: left;
}

ul li, ol li {
  margin-bottom: 0.5rem;
}

/* 🎛️ Buttons */
button {
  background-color: #b2541c;
  color: #fff;
  padding: 0.5rem 1rem;
  border: none;
  border-radius: 8px;
  cursor: pointer;
}

button:hover {
  background-color: #a0522d;
}

/* 📱 Responsive Tweaks */
@media screen and (max-width: 768px) {
  .column {
    flex: 1 1 100%;
  }

  .main-header h1 {
    font-size: 2rem;
  }

  .main-footer p {
    font-size: 0.85rem;
  }
}
