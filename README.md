<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ubuntu Eats</title>
    <style>
        body {
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
        }
        .container {
            max-width: 800px;
            margin: auto;
        }
        h1 {

            font-size: 3em;
        }
        p {
            font-size: 1.2em;
        }
        .menu, .reserve, .trading-hours {
            margin-top: 20px;
            padding: 10px;
            border: 1px solid white;
            text-align: left;
        }
        .contact {
            margin-top: 20px;
            font-size: 1.2em;
        }
        .address {
            margin-top: 40px;
            font-size: 1em;
        }
        .menu-content, .reserve-content {
            display: none;

        }
        .menu h2, .reserve h2 {
            cursor: pointer;
        }
    </style>
    <script>
        function toggleMenu() {
            var menuContent = document.getElementById("menu-content");
            if (menuContent.style.display === "none" || menuContent.style.display === "") {
                menuContent.style.display = "block";
            } else {
                menuContent.style.display = "none";
            }
        }
        function toggleReserve() {
            var reserveContent = 

document.getElementById("reserve-content");
            if (reserveContent.style.display === "none" || reserveContent.style.display === "") {
                reserveContent.style.display = "block";
            } else {
                reserveContent.style.display = "none";
            }
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>Ubuntu Eats</h1>
        <p>Welcome to Ubuntu Eats, where flavor meets community.</p>
        <div class="menu">
            <h2 onclick="toggleMenu()">Ubuntu 

Eats Sushi & Grill Menu ▼</h2>
            <div id="menu-content" class="menu-content">
                <h3>Appetizers</h3>
                <ul>
                    <li>Edamame - Steamed soybeans with sea salt</li>
                    <li>Miso Soup - Traditional miso with tofu, seaweed, and scallions</li>
                    <li>Gyoza - Pan-seared dumplings with a savory filling</li>
                    <li>Tempura - Lightly battered shrimp and vegetables</li>
                    <li>Takoyaki - Octopus-filled dough balls drizzled with savory sauce</li>
                </ul>
                <h3>Sushi Rolls</h3>
                <ul>
                    <li>California Roll - Crab, avocado, and cucumber</li>
                    <li>Spicy Tuna Roll - Tuna, spicy 

mayo, and scallions</li>
                    <li>Dragon Roll - Eel, avocado, cucumber, and eel sauce</li>
                    <li>Rainbow Roll - Assorted sashimi over a California roll</li>
                    <li>Volcano Roll - Spicy crab, cucumber, and baked seafood topping</li>
                </ul>
                <h3>Sashimi & Nigiri</h3>
                <ul>
                    <li>Salmon (Sake)</li>
                    <li>Tuna (Maguro)</li>
                    <li>Yellowtail (Hamachi)</li>
                    <li>Shrimp (Ebi)</li>
                    <li>Octopus (Tako)</li>
                </ul>
            </div>
        </div>
        <div class="reserve">
            <h2 onclick="toggleReserve()">Reserve a Table 

▼</h2>
            <div id="reserve-content" class="reserve-content">
                <form>
                    <label for="party">Party Size:</label>
                    <input type="number" id="party" name="party" min="1" max="20" required>
                    <br>
                    <label for="date">Date:</label>
                    <input type="date" id="date" name="date" min="2025-01-01" max="2025-12-31" required>
                    <br>
                    <label for="time">Time:</label>
                    <select id="time" name="time" required>
                        <option value="11:00">11:00 AM</option>
                        <option value="12:00">12:00 PM</option>

                        <option value="13:00">1:00 PM</option>
                        <option value="14:00">2:00 PM</option>
                        <option value="15:00">3:00 PM</option>
                        <option value="16:00">4:00 PM</option>
                        <option value="17:00">5:00 PM</option>
                        <option value="18:00">6:00 PM</option>
                        <option value="19:00">7:00 PM</option>
                        <option value="20:00">8:00 PM</option>
                        <option value="21:00">9:00 PM</option>
                    </select>
                    <br>
                    <button 

type="submit">Reserve</button>
                </form>
            </div>
        </div>
        <div class="trading-hours">
            <h2>Trading Hours</h2>
            <p>Monday: 11 am–9 pm</p>
            <p>Tuesday: 11 am–9:45 pm</p>
            <p>Wednesday: 11 am–9:45 pm</p>
            <p>Thursday: 11 am–9:45 pm</p>
            <p>Friday: 11 am–9:45 pm</p>
            <p>Saturday: 11 am–9:45 pm</p>
            <p>Sunday: 11 am–9 pm</p>
        </div>
        <div class="contact">
            <h2>Contact Us</h2>
            <p>Phone: +27633948869</p>
        </div>
        <div class="address">
            <p>Ubuntu Eats, Shop No 20 of Nelson Mandela Square, Corner Maude & 

5th St, Sandton, 2016</p
