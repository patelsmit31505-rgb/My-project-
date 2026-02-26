const express = require("express");
const app = express();

app.use(express.static("public"));

app.get("/", (req, res) => {
  res.send("App is Live 🚀");
});

const PORT = process.env.PORT || 3000;
app.listen(PORT, "0.0.0.0", () => {
  console.log("Server running");
});
{
  "name": "app",
  "version": "1.0.0",
  "main": "server.js",
  "scripts": {
    "start": "node server.js"
  },
  "dependencies": {
    "express": "^4.18.2"
  }
}
<h1>🔥 Your App is Live</h1>
