# financial-dashboard
My Financial Dashboard Website
import React, { useEffect, useState } from "react";
import axios from "axios";

function Dashboard() {
  const [data, setData] = useState({});

  useEffect(() => {
    axios.get("/api/summary")
      .then(res => setData(res.data));
  }, []);

  return (
    <div>
      <h1>Financial Dashboard</h1>
      <p>Revenue: ${data.revenue}</p>
      <p>Expenses: ${data.expenses}</p>
      <p>Profit: ${data.profit}</p>
    </div>
  );
}

export default Dashboard;
