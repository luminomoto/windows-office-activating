# windows-office-activating
In this tutorial, I will show you how to activate Windows and Office tools using only PowerShell.

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Activate Windows</title>
  <style>
    body { font-family: sans-serif; padding: 2rem; }
    .code-box {
      background: #f4f4f4;
      border-radius: 8px;
      padding: 1rem;
      position: relative;
      font-family: monospace;
    }
    button {
      position: absolute;
      top: 10px;
      right: 10px;
      padding: 0.4rem 0.8rem;
      border: none;
      border-radius: 5px;
      background-color: #007acc;
      color: white;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <h1>How to Activate Windows</h1>
  <div class="code-box">
    <code id="cmd">irm https://get.activated.win | iex</code>
    <button onclick="copyText()">Copy</button>
  </div>

  <script>
    function copyText() {
      const text = document.getElementById("cmd").innerText;
      navigator.clipboard.writeText(text).then(() => {
        alert("Copied!");
      });
    }
  </script>

</body>
</html>
