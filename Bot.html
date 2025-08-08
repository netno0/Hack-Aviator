<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aviator Signal Predictor</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&amp;display=swap" rel="stylesheet">
    <style>
      body {
        font-family: "Montserrat", sans-serif;
        background-color: #121212;
        color: white;
        text-align: center;
        margin: 0;
        padding: 20px;
        min-height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
      }

      .game-container {
        max-width: 600px;
        width: 100%;
        margin: 0 auto;
        background-color: #1e1e1e;
        border-radius: 15px;
        padding: 25px;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        transform: translateY(0);
        transition: transform 0.3s ease;
      }

      .game-container:hover {
        transform: translateY(-5px);
      }

      h1 {
        color: #ffcc00;
        margin-bottom: 25px;
        font-weight: 600;
        text-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
      }

      .aviator-display {
        height: 200px;
        background-color: #2a2a2a;
        border-radius: 10px;
        margin: 25px 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        position: relative;
        overflow: hidden;
      }

      .multiplier {
        font-size: 47px;
        font-weight: 600;
        color: #00cc66;
        margin-bottom: 20px;
        text-shadow: 0 0 10px rgba(0, 204, 102, 0.5);
        animation: float 3s ease-in-out infinite;
      }

      .plane {
        font-size: 40px;
        position: absolute;
        left: 0;
        top: 50%;
        transform: translateY(-50%);
        transition: left 0.05s linear;
      }

      .history-container {
        max-height: 90px;
        overflow-y: auto;
        margin-bottom: 25px;
        padding: 10px;
        background-color: #2a2a2a;
        border-radius: 10px;
      }

      .history {
        display: flex;
        flex-direction: column;
        gap: 8px;
      }

      .history-item {
        padding: 10px;
        border-radius: 8px;
        display: flex;
        justify-content: space-between;
        background-color: rgba(255, 204, 0, 0.1);
        border-left: 4px solid #ffcc00;
      }

      .history-multiplier {
        font-weight: 600;
        color: #ffcc00;
      }

      .history-result {
        font-weight: 600;
      }

      .success {
        color: #00cc66;
      }

      .fail {
        color: #ff4444;
      }

      .controls {
        margin-top: 30px;
        display: flex;
        justify-content: center;
        gap: 20px;
      }

      button {
        background-color: #ffcc00;
        color: #121212;
        border: none;
        padding: 14px 30px;
        border-radius: 8px;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s ease;
        font-size: 16px;
        letter-spacing: 0.5px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        position: relative;
        overflow: hidden;
        width: 200px;
      }

      button:hover {
        background-color: #ffdd33;
        transform: translateY(-3px);
        box-shadow: 0 7px 14px rgba(0, 0, 0, 0.2);
      }

      button:active {
        transform: translateY(1px);
      }

      button::after {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(
          45deg,
          transparent 25%,
          rgba(255, 255, 255, 0.1) 50%,
          transparent 75%
        );
        background-size: 400% 400%;
        opacity: 0;
        transition: all 0.5s ease;
      }

      button:hover::after {
        opacity: 1;
        animation: shine 1.5s infinite;
      }

      input {
        padding: 10px 20px;
        border-radius: 8px;
        background-color: #333;
        color: white;
        border: none;
        font-size: 16px;
        cursor: text;
        transition: all 0.3s ease;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        width: 200px;
        text-align: center;
      }

      input:invalid {
        border: 2px solid #ff4444;
      }

      input:valid {
        border: 2px solid #00cc66;
      }

      input:hover {
        background-color: #444;
      }

      label {
        display: block;
        margin-bottom: 8px;
        font-weight: 600;
        color: #ddd;
      }

      .hidden {
        display: none;
      }

      .id-form {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 20px;
        margin-bottom: 30px;
      }

      @keyframes pulse {
        0% {
          transform: scale(1);
        }
        100% {
          transform: scale(1.05);
        }
      }

      @keyframes float {
        0% {
          transform: translateY(0px);
        }
        50% {
          transform: translateY(-5px);
        }
        100% {
          transform: translateY(0px);
        }
      }

      @keyframes shine {
        0% {
          background-position: 100% 50%;
        }
        100% {
          background-position: 0% 50%;
        }
      }

      .error-message {
        color: #ff4444;
        margin-top: 5px;
        font-size: 14px;
        height: 20px;
      }

      /* Scrollbar styles */
      ::-webkit-scrollbar {
        width: 8px;
      }

      ::-webkit-scrollbar-track {
        background: #1e1e1e;
        border-radius: 4px;
      }

      ::-webkit-scrollbar-thumb {
        background: #ffcc00;
        border-radius: 4px;
      }

      ::-webkit-scrollbar-thumb:hover {
        background: #ffdd33;
      }
    </style>
  </head>
  <body>
    <div class="game-container">
      <h1>Aviator Signal Predictor</h1>

      <div class="id-form" id="id-form">
        <div class="setting-group">
          <label for="user-id">Enter YOUR Betwinner ID</label>
          <input type="text" id="user-id" pattern="\d{8,}" inputmode="numeric" placeholder="Your Betwinner ID" required="" title="Please enter at least 8 digits">
          <div class="error-message" id="error-message"></div>
        </div>
        <button id="verify-btn">Verify ID</button>
      </div>

      <div id="game-content" class="hidden">
        <div class="aviator-display">
          <div class="multiplier" id="multiplier">GET YOUR SIGNAL</div>
        </div>

        <div class="history-container">
          <div class="history" id="history">
            <!-- History items will be added here -->
          </div>
        </div>

        <div class="controls">
          <button id="predict-btn" onclick="getPrediction()">
            <span>Get Signal</span>
          </button>
        </div>
      </div>
    </div>

    <script>
      // DOM elements
      const idForm = document.getElementById("id-form");
      const gameContent = document.getElementById("game-content");
      const userIdInput = document.getElementById("user-id");
      const verifyBtn = document.getElementById("verify-btn");
      const errorMessage = document.getElementById("error-message");
      const multiplierElement = document.getElementById("multiplier");
      const historyElement = document.getElementById("history");
      const predictButton = document.getElementById("predict-btn");

      // Game state
      const gameState = {
        userId: null,
        currentMultiplier: 0,
        predictionMultiplier: 0,
        history: [],
        isRunning: false,
      };

      // Verify ID button handler
      verifyBtn.addEventListener("click", () => {
        // Validate input
        if (userIdInput.validity.valid) {
          gameState.userId = userIdInput.value;
          idForm.classList.add("hidden");
          gameContent.classList.remove("hidden");
          errorMessage.textContent = "";
        } else {
          if (userIdInput.value.length < 8) {
            errorMessage.textContent = "ID must be at least 8 digits";
          } else if (!/^\d+$/.test(userIdInput.value)) {
            errorMessage.textContent = "ID must contain only numbers";
          } else {
            errorMessage.textContent = "Invalid ID format";
          }
        }
      });

      // Force numeric input
      userIdInput.addEventListener("input", function () {
        this.value = this.value.replace(/\D/g, "");
        errorMessage.textContent = "";
      });

      // Generate new prediction with faster animation
      function getPrediction() {
        if (gameState.isRunning) return;

        // Disable button during animation
        predictButton.disabled = true;
        predictButton.textContent = "AI Analysing...";
        multiplierElement.textContent = "1.00";
        multiplierElement.style.color = "#00cc66";

        // Generate random crash multiplier (1.50x to 10.00x)
        const crashMultiplier = (1.5 + Math.random() * 8.5).toFixed(2);

        // Generate prediction (slightly before crash)
        const predictionMultiplier = Math.max(
          1.2,
          (crashMultiplier - 0.5 - Math.random() * 0.7).toFixed(2)
        );
        gameState.predictionMultiplier = predictionMultiplier;

        // Start animation
        gameState.isRunning = true;
        let currentPos = 0;
        const crashPos = ((crashMultiplier - 1) / 9) * 100; // Convert 1-10 to 0-100%
        const predictPos = ((predictionMultiplier - 1) / 9) * 100;

        // Faster animation interval (50ms instead of 100ms)
        const interval = setInterval(() => {
          currentPos += 1.5; // Increased speed

          // Update multiplier display
          const currentMultiplier = (1 + (currentPos / 100) * 9).toFixed(2);
          multiplierElement.textContent = currentMultiplier + " x";

          // Highlight when reach prediction point
          if (currentPos >= predictPos) {
            multiplierElement.style.color = "#ffcc00";
          }

          // Check for crash
          if (currentPos >= crashPos) {
            clearInterval(interval);
            gameState.isRunning = false;
            multiplierElement.textContent = predictionMultiplier + " x";
            multiplierElement.style.color = "#00cc66";

            // Add to history (all results saved)
            addToHistory(predictionMultiplier, crashMultiplier);

            // Re-enable button after delay
            setTimeout(() => {
              predictButton.disabled = false;
              predictButton.textContent = "Get Signal";
            }, 1000);
          }
        }, 50); // Faster interval
      }

      // Add result to history (all results saved)
      function addToHistory(prediction, crash) {
        const success = parseFloat(crash) >= parseFloat(prediction);
        const historyItem = document.createElement("div");
        historyItem.className = "history-item";

        historyItem.innerHTML = `
          <span class="history-multiplier">${prediction}x</span>
          <span class="history-result ${success ? "success" : "fail"}">
            ${success ? "CASH OUT" : ""}
          </span>
        `;

        // Add to beginning
        historyElement.insertBefore(historyItem, historyElement.firstChild);
      }
    </script>
  

</body>
