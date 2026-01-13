<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>APEX – Smart Healthcare Platform</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #f4f6f9;
}

header {
    background: #0d6efd;
    color: white;
    padding: 20px;
    text-align: center;
}

.container {
    padding: 20px;
}

.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 15px;
}

.card {
    background: white;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.08);
}

.card h3 {
    margin-top: 0;
    color: #0d6efd;
}

.status {
    font-size: 22px;
    font-weight: bold;
}

.green { color: green; }
.red { color: red; }
.orange { color: orange; }

.section {
    margin-top: 30px;
}

table {
    width: 100%;
    border-collapse: collapse;
}

table th, table td {
    padding: 10px;
    border-bottom: 1px solid #ddd;
    text-align: left;
}

button {
    padding: 10px 15px;
    background: #0d6efd;
    border: none;
    color: white;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background: #084298;
}

footer {
    text-align: center;
    padding: 15px;
    background: #e9ecef;
    margin-top: 40px;
}
</style>
</head>

<body>

<header>
    <h1>APEX – Smart Healthcare Management System</h1>
    <p>AI Powered | City-wide | Emergency Ready</p>
</header>

<div class="container">

    <!-- Dashboard Cards -->
    <div class="grid">
        <div class="card">
            <h3>OPD Queue</h3>
            <p class="status orange" id="opd">42 Patients Waiting</p>
        </div>

        <div class="card">
            <h3>Emergency Beds</h3>
            <p class="status green" id="beds">12 Beds Available</p>
        </div>

        <div class="card">
            <h3>ICU Status</h3>
            <p class="status red">90% Occupied</p>
        </div>

        <div class="card">
            <h3>Inventory Alerts</h3>
            <p class="status orange">3 Medicines Expiring</p>
        </div>
    </div>

    <!-- City Hospitals -->
    <div class="section">
        <h2>🏥 City-wide Hospital Integration</h2>
        <table>
            <tr>
                <th>Hospital</th>
                <th>OPD Load</th>
                <th>Emergency Beds</th>
            </tr>
            <tr>
                <td>City General Hospital</td>
                <td>High</td>
                <td>2</td>
            </tr>
            <tr>
                <td>Metro Care Center</td>
                <td>Medium</td>
                <td>5</td>
            </tr>
            <tr>
                <td>LifeLine Hospital</td>
                <td>Low</td>
                <td>5</td>
            </tr>
        </table>
    </div>

    <!-- Patient Feedback -->
    <div class="section">
        <h2>💬 Patient Feedback</h2>
        <div class="card">
            <p>⭐ ⭐ ⭐ ⭐ ☆</p>
            <p>“Virtual OPD saved my waiting time.”</p>
        </div>
    </div>

    <!-- Action -->
    <div class="section">
        <button onclick="updateData()">Simulate Live Update</button>
    </div>

</div>

<footer>
    <p>APEX ©️ 2026 | Smart City Healthcare Platform</p>
</footer>

<script>
function updateData() {
    document.getElementById("opd").innerText =
        Math.floor(Math.random() * 60) + " Patients Waiting";
    document.getElementById("beds").innerText =
        Math.floor(Math.random() * 15) + " Beds Available";
}
</script>

</body>
</html>
