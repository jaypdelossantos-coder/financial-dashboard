<!DOCTYPE html>
<html>
<head>
<title>Financial Dashboard</title>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</head>

<body>

<h1>Financial Dashboard</h1>

<h3>Revenue: $50,000</h3>
<h3>Expenses: $32,000</h3>
<h3>Profit: $18,000</h3>

<canvas id="myChart"></canvas>

<script>
const ctx = document.getElementById('myChart');

new Chart(ctx, {
 type: 'line',
 data: {
  labels: ['Jan','Feb','Mar','Apr'],
  datasets: [{
   label: 'Revenue',
   data: [12000,15000,10000,20000],
   borderColor: 'green'
  }]
 }
});
</script>

</body>
</html>
<!DOCTYPE html>
<html>

<head>
<title>Financial Dashboard</title>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</head>

<body>

<h1>Financial Dashboard</h1>

<h3>Total Revenue: $50,000</h3>
<h3>Total Expenses: $32,000</h3>
<h3>Net Profit: $18,000</h3>

<h2>Revenue Chart</h2>

<canvas id="revenueChart"></canvas>

<script>
const ctx = document.getElementById('revenueChart');

new Chart(ctx, {
 type: 'bar',
 data: {
  labels: ['Jan','Feb','Mar','Apr','May','Jun'],
  datasets: [{
   label: 'Revenue',
   data: [12000,15000,10000,20000,18000,22000],
   backgroundColor: 'green'
  }]
 }
});
</script>

</body>
</html>
<h2>Expense Breakdown</h2>

<canvas id="expenseChart" width="400" height="200"></canvas>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script>
const expenseCtx = document.getElementById('expenseChart');

new Chart(expenseCtx, {
    type: 'pie',
    data: {
        labels: [
            'Salaries',
            'Rent',
            'Utilities',
            'Marketing',
            'Supplies'
        ],
        datasets: [{
            label: 'Expenses',
            data: [15000, 5000, 2000, 3000, 1000],
            backgroundColor: [
                '#FF6384',
                '#36A2EB',
                '#FFCE56',
                '#4CAF50',
                '#9C27B0'
            ],
            borderWidth: 1
        }]
    },
    options: {
        responsive: true,
        plugins: {
            title: {
                display: true,
                text: 'Company Expense Distribution'
            },
            legend: {
                position: 'bottom'
            }
        }
    }
});
</script>
<h1>Financial Dashboard</h1>

<h3>Total Revenue: $50,000</h3>
<h3>Total Expenses: $32,000</h3>
<h3>Net Profit: $18,000</h3>

<h2>Revenue Chart</h2>
<canvas id="revenueChart"></canvas>

<h2>Expense Breakdown</h2>
<canvas id="expenseChart"></canvas>
