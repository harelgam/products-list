<!DOCTYPE html>
<html lang="he">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>רשימת הקניות שלך</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            margin: 0;
            padding: 20px;
            direction: rtl; /* Right-to-left text direction for Hebrew content */
        }

        .cart-container {
            max-width: 800px;
            margin: 0 auto;
            background-color: #fff;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            overflow: auto; /* Enable scrolling if needed */
            max-height: 80vh; /* Limit the height of the container */
        }

        ul {
            padding: 0;
            list-style-type: none;
        }

        li {
            padding: 10px 0;
            border-bottom: 1px solid #ccc; /* Add a border between items */
            cursor: pointer; /* Change cursor to pointer on hover for clickable effect */
        }

        li.active {
            background-color: #f9f9f9; /* Highlight background color for active item */
        }
    </style>
</head>
<body>
    <div class="cart-container">
        <h1>מוצרים בסל הקניות שלך</h1>
        <ul>
            <li>חלב</li>
        <li>ביצים</li>
        <li>לחם</li>
        <li>גבינה</li>
        <li>עוף</li>
        <li>אורז</li>
        <li>פסטה</li>
        <li>תפוחים</li>
        <li>תפוזים</li>
        <li>בננות</li>
        <li>גזרים</li>
        <li>חסה</li>
        <li>עגבניות</li>
        <li>בצלים</li>
        <li>תפוחי אדמה</li>
        <li>יוגורט</li>
        <li>חמאה</li>
        <li>דגני בוקר</li>
        <li>קְוֵקֶר</li>
        <li>תה</li>
        <li>קפה</li>
        <li>סוכר</li>
        <li>קמח</li>
        <li>מלח</li>
        <li>פלפל</li>
        <li>קטשופ</li>
        <li>חרדל</li>
        <li>מיונז</li>
        <li>רוטב לסלט</li>
        <li>שמן זית</li>
        <li>חומץ</li>
        <li>שימורי שעועית</li>
        <li>עגבניות משומרות</li>
        <li>חמאת בוטנים</li>
        <li>ג'לי</li>
        <li>פרורי לחם</li>
        <li>מרק</li>
        <li>מרק בשר</li>
        <li>קוביות חמין</li>
        <li>קרקרים</li>
        <li>צ'יפס</li>
        <li>סלסה</li>
        <li>גואקמולי</li>
        <li>טורטיות</li>
        <li>חציות גלידה</li>
        <li>ארוחות ערב קפואות</li>
        <li>פיצה</li>
        <li>נקניקיות</li>
        <li>קציצות המבורגר</li>
        <li>לחמניות</li>
            <!-- Include all other products here -->
        </ul>
    </div>
    
    <script>
        const listItems = document.querySelectorAll('li');

        listItems.forEach(item => {
            item.addEventListener('click', () => {
                // Remove 'active' class from all items
                listItems.forEach(li => li.classList.remove('active'));
                
                // Add 'active' class to the clicked item
                item.classList.add('active');
                
                // Show a message box with the selected product name
                alert("המוצר " + item.textContent.trim() + " נבחר");
            });
        });
    </script>
</body>
</html>

