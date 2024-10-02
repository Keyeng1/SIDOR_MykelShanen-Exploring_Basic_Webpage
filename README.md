# SIDOR_MykelShanen-Exploring_Data_Dashboard
<html>
<head>
    <title>Basic Data Dashboard</title>
    <style>
        body {
            background-color: #f0f0f0;
            font-family: Arial, sans-serif;
        }

        header {
            background-color: #333;
            color: white;
            padding: 10px;
            text-align: center;   

        }

        main {
            padding: 20px;
            text-align: center;
        }

        .metric {
            background-color: white;
            border: 1px solid #ccc;
            margin: 10px;
            padding: 10px;
        }

        button {
            background-color: #4CAF50;
            border: none;
            color: white;
            padding: 10px 20px;
            text-align: center;
            text-decoration:   
 none;
            display: inline-block;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
        }

        button:hover {
            background-color: #3e8e41;
        }
    </style>
</head>
<body>   

    <header>
        <h1>Basic Data Dashboard</h1>
    </header>
    <main>
        <section>
            <h2>Key Metrics</h2>
            <div class="metric">
                <p>Total Users: <span id="totalUsers">1000</span></p>
            </div>
            <div class="metric">
                <p>Total Sales: <span id="totalSales">500</span></p>
            </div>
            <button id="alertButton">Show Alert</button>
        </section>
    </main>
    <footer>
        &copy; 2024 Your Name
    </footer>
    <script>
        const totalUsersElement = document.getElementById('totalUsers');
        const totalSalesElement = document.getElementById('totalSales');
        const alertButton = document.getElementById('alertButton');

        alertButton.addEventListener('click', () => {
            const totalUsers = parseInt(totalUsersElement.textContent);
            const totalSales = parseInt(totalSalesElement.textContent);
            alert(`Total Users: ${totalUsers}, Total Sales: ${totalSales}`);
        });
    </script>
</body>
</html>
