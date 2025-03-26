<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simulator Deposito BPR Penataran</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --primary: #2563eb;
            --secondary: #1d4ed8;
            --accent: #3b82f6;
            --dark: #1e293b;
            --light: #f8fafc;
            --success: #10b981;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background: #f1f5f9;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 1rem;
        }
        
        .container {
            background: white;
            border-radius: 1rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 28rem;
            padding: 2rem;
        }
        
        .header {
            text-align: center;
            margin-bottom: 1.5rem;
        }
        
        .header h1 {
            color: var(--primary);
            font-size: 1.5rem;
            font-weight: 600;
            line-height: 1.2;
        }
        
        .header .icon {
            font-size: 1.75rem;
            margin-bottom: 0.5rem;
            color: var(--primary);
        }
        
        .input-group {
            margin-bottom: 1.25rem;
        }
        
        label {
            display: block;
            margin-bottom: 0.5rem;
            color: var(--dark);
            font-weight: 500;
            font-size: 0.875rem;
        }
        
        input, select {
            width: 100%;
            padding: 0.75rem 1rem;
            border: 1px solid #e2e8f0;
            border-radius: 0.5rem;
            font-size: 0.875rem;
            transition: all 0.2s;
        }
        
        input:focus, select:focus {
            border-color: var(--accent);
            box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.1);
            outline: none;
        }
        
        button {
            width: 100%;
            padding: 0.75rem;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 0.5rem;
            font-size: 0.875rem;
            font-weight: 500;
            cursor: pointer;
            transition: all 0.2s;
            margin-top: 0.5rem;
        }
        
        button:hover {
            background: var(--secondary);
        }
        
        .result {
            margin-top: 1.5rem;
            padding: 1.25rem;
            background: #f8fafc;
            border-radius: 0.75rem;
            border-left: 4px solid var(--success);
            display: none;
        }
        
        .result h3 {
            color: var(--dark);
            margin-bottom: 1rem;
            font-size: 1rem;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        
        .result-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 0.75rem;
            padding-bottom: 0.75rem;
            border-bottom: 1px dashed #e2e8f0;
            font-size: 0.875rem;
        }
        
        .result-item:last-child {
            border-bottom: none;
            font-weight: 600;
            color: var(--primary);
        }
        
        .note {
            margin-top: 1.5rem;
            font-size: 0.75rem;
            color: #64748b;
            text-align: center;
            line-height: 1.5;
        }
        
        .error {
            color: #ef4444;
            font-size: 0.75rem;
            margin-top: 0.25rem;
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="icon"><i class="fas fa-calculator"></i></div>
            <h1>Simulator Deposito<br>BPR Penataran</h1>
        </div>
        
        <div class="input-group">
            <label for="amount">Dana Deposito Awal</label>
            <input type="text" id="amount" placeholder="Contoh: 10.000.000" oninput="formatRupiah(this)">
            <div class="error" id="amount-error">Minimal Rp1.000.000</div>
        </div>
        
        <div class="input-group">
            <label for="tenor">Tenor Deposito</label>
            <select id="tenor">
                <option value="1">1 Bulan</option>
                <option value="3">3 Bulan</option>
                <option value="6">6 Bulan</option>
                <option value="12">12 Bulan</option>
            </select>
        </div>
        
        <div class="input-group">
            <label for="interest">Bunga Deposito (% per tahun)</label>
            <input type="text" id="interest" placeholder="Contoh: 6,25" oninput="formatPercentage(this)">
        </div>
        
        <button onclick="calculate()">Hitung Sekarang</button>
        
        <div class="result" id="result">
            <h3><i class="fas fa-chart-line"></i> Hasil Perhitungan</h3>
            <div class="result-item">
                <span>Bunga (Sebelum Pajak)</span>
                <span id="gross-interest">Rp0</span>
            </div>
            <div class="result-item">
                <span>Pajak (20%)</span>
                <span id="tax">Rp0</span>
            </div>
            <div class="result-item">
                <span>Bunga (Setelah Pajak)</span>
                <span id="net-interest">Rp0</span>
            </div>
            <div class="result-item">
                <span>Total Dana Akhir</span>
                <span id="total">Rp0</span>
            </div>
        </div>
        
        <div class="note">
            *Simulasi ini hanya perkiraan. Untuk informasi lebih lanjut,<br>
            hubungi Customer Service BPR Penataran.
        </div>
    </div>

    <script>
        function formatRupiah(input) {
            let value = input.value.replace(/\D/g, "");
            if (value === "") {
                input.value = "";
                return;
            }
            let number = parseInt(value);
            input.value = new Intl.NumberFormat("id-ID").format(number);
            
            document.getElementById("amount-error").style.display = 
                (number < 1000000 && number > 0) ? "block" : "none";
        }
        
        function formatPercentage(input) {
            let value = input.value.replace(/[^0-9,]/g, "").replace(/,/g, ".");
            if (value === "") {
                input.value = "";
                return;
            }
            input.value = value.replace(".", ",");
        }
        
        function calculate() {
            const amountStr = document.getElementById("amount").value.replace(/\./g, "");
            const amount = parseFloat(amountStr) || 0;
            const tenor = parseInt(document.getElementById("tenor").value);
            const interestStr = document.getElementById("interest").value.replace(/,/g, ".");
            const interestRate = parseFloat(interestStr) || 0;
            
            if (amount < 1000000) {
                alert("Minimal deposito Rp1.000.000");
                return;
            }
            
            if (interestRate <= 0) {
                alert("Masukkan suku bunga yang valid (contoh: 6,25)");
                return;
            }
            
            const grossInterest = Math.round((amount * (interestRate / 100) * tenor / 12));
            const tax = Math.round(grossInterest * 0.20);
            const netInterest = grossInterest - tax;
            const total = amount + netInterest;
            
            document.getElementById("gross-interest").textContent = "Rp" + grossInterest.toLocaleString("id-ID");
            document.getElementById("tax").textContent = "Rp" + tax.toLocaleString("id-ID");
            document.getElementById("net-interest").textContent = "Rp" + netInterest.toLocaleString("id-ID");
            document.getElementById("total").textContent = "Rp" + total.toLocaleString("id-ID");
            
            document.getElementById("result").style.display = "block";
        }
    </script>
</body>
</html>
