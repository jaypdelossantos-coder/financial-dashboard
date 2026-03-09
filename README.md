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
