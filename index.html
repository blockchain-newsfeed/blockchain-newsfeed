<html lang="en">
    <meta charset="UTF-8">
    <meta name="viewport">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap" rel="stylesheet">
    <style>
        #tokenDataTable {
            font-family: 'Poppins', sans-serif;
            overflow-y: auto;
            max-height: 300px;
        }
        #tokenDataTable table {
            width: 100%;
            table-layout: fixed; /* Add this line */
        }
        #tokenDataTable th, #tokenDataTable td {
            text-align: left;
            padding: 8px;
        }
        #tokenDataTable th {
            position: sticky;
            top: 0;
            background-color: #4237FF;
            color: white;
            z-index: 2; /* Ensure it stays on top of other content */
        }
        #tokenDataTable tr:nth-child(even) {
            background-color: #F2F2F2;
        }
        #tokenDataTable tr:nth-child(odd) {
            background-color: #FFFFFF;
        }
        #tokenDataTable .positive {
            color: green;
        }
        #tokenDataTable .negative {
            color: red;
        }
    </style>
<body>
    <div id="tokenDataTable">
        <table>
            <thead>
                <tr>
                    <th>Symbol</th>
                    <th>Price</th>
                    <th>24h Change</th>
                    <th>Market Cap</th>
                </tr>
            </thead>
            <tbody>
                <!-- The rows will be added here by the loadData() function -->
            </tbody>
        </table>
    </div>
    <script>
        async function loadData() {
            const apiUrl = 'https://api.coingecko.com/api/v3/search/trending';
            const tbody = document.querySelector('#tokenDataTable tbody');
            try {
                const response = await fetch(apiUrl);
                let {coins} = await response.json();
                // Sort coins by price change percentage 24h
                coins.sort((a, b) => b.item.data.price_change_percentage_24h.usd - a.item.data.price_change_percentage_24h.usd);
                coins.forEach(({item}) => {
                    const row = tbody.insertRow(-1);
                    const symbolCell = row.insertCell(0);
                    const priceCell = row.insertCell(1);
                    const changeCell = row.insertCell(2);
                    const marketCapCell = row.insertCell(3);
                    symbolCell.innerHTML = item.symbol.toUpperCase();
                    priceCell.innerHTML = item.data.price;
                    changeCell.innerHTML = `${item.data.price_change_percentage_24h.usd.toFixed(2)}%`;
                    changeCell.className = item.data.price_change_percentage_24h.usd > 0 ? 'positive' : 'negative';
                    marketCapCell.innerHTML = item.data.market_cap;
                });
            } catch (error) {
                console.error('Error:', error);
                const row = tbody.insertRow(-1);
                const cell = row.insertCell(0);
                cell.innerHTML = 'Error loading data.';
                cell.colSpan = 4;
            }
        }
        loadData(); // Call loadData function immediately after defining it
    </script>
</body>
</html>
