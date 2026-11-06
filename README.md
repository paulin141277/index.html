<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stock and Inventory Mini-App</title>
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body { font-family: Arial, sans-serif; background-color: #f4f6f8; margin: 0; padding: 0; }
        header { background-color: #00897b; color: white; padding: 16px; font-size: 18px; font-weight: bold; text-align: center; }
        .dashboard { padding: 16px; display: grid; grid-template-columns: 1fr 1fr; gap: 12px; max-width: 600px; margin: auto; }
        .card { background-color: #00897b; color: white; padding: 20px; border-radius: 8px; text-align: center; cursor: pointer; box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
        .card.full { grid-column: span 2; }
        .card h3 { margin: 0 0 8px 0; font-size: 16px; }
        .card p { margin: 0; font-size: 14px; opacity: 0.9; }
    </style>
</head>
<body>
    <header>Stock and Inventory</header>
    <div class="dashboard">
        <div class="card full" onclick="alert('Menu Goods dibuka')">
            <h3>Goods</h3>
            <p id="stock-count">Total Stok: 870</p>
        </div>
        <div class="card" onclick="alert('Menu Documents dibuka')">
            <h3>Documents</h3>
            <p>68 Dokumen</p>
        </div>
        <div class="card" onclick="alert('Menu Reports dibuka')">
            <h3>Reports</h3>
            <p>Lihat Grafik</p>
        </div>
        <div class="card" onclick="alert('Menu Settings dibuka')">
            <h3>Settings</h3>
            <p>Pengaturan</p>
        </div>
        <div class="card" onclick="alert('Menu Bantuan dibuka')">
            <h3>Bantuan</h3>
            <p>Panduan</p>
        </div>
    </div>
    <script>
        let tg = window.Telegram.WebApp;
        tg.expand();
    </script>
</body>
</html># index.html
