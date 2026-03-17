# Problem 6 – Curve Length and Numerical Integration

We are given the parametric curve

- x(t) = t
- y(t) = t^2
- t in [0, 1]

We solve the problem step by step.

---

## 1. Position vector

The position vector is

r(t) = (x(t), y(t)) = (t, t^2)

---

## 2. Velocity vector

The velocity vector is the derivative of the position vector:

v(t) = dr/dt

Differentiate each component:

- d/dt[t] = 1
- d/dt[t^2] = 2t

So,

v(t) = (1, 2t)

---

## 3. Magnitude of the velocity

The speed is the magnitude of the velocity vector:

|v(t)| = sqrt(1^2 + (2t)^2)

So,

|v(t)| = sqrt(1 + 4t^2)

---

## 4. Arc length as an integral

The arc length of a parametric curve from t = 0 to t = 1 is

s = ∫_0^1 |v(t)| dt

Substitute |v(t)|:

s = ∫_0^1 sqrt(1 + 4t^2) dt

So the arc length integral is

s = ∫_0^1 sqrt(1 + 4t^2) dt

---

## 5. Analytical calculation of the integral

We compute

s = ∫_0^1 sqrt(1 + 4t^2) dt

Use the substitution

u = 2t

Then

du = 2 dt
dt = du / 2

Also:

- when t = 0, u = 0
- when t = 1, u = 2

So the integral becomes

s = ∫_0^2 sqrt(1 + u^2) · (1/2) du

Therefore,

s = (1/2) ∫_0^2 sqrt(1 + u^2) du

Now use the standard formula

∫ sqrt(1 + u^2) du = (1/2)u sqrt(1 + u^2) + (1/2) ln(u + sqrt(1 + u^2)) + C

So,

s = (1/2) * [ (1/2)u sqrt(1 + u^2) + (1/2) ln(u + sqrt(1 + u^2)) ] from 0 to 2

Simplify the factor:

s = (1/4) [ u sqrt(1 + u^2) + ln(u + sqrt(1 + u^2)) ] from 0 to 2

Now evaluate at u = 2:

- sqrt(1 + 2^2) = sqrt(5)

So the upper value is

2sqrt(5) + ln(2 + sqrt(5))

Now evaluate at u = 0:

- sqrt(1 + 0^2) = 1
- ln(0 + 1) = ln(1) = 0

So the lower value is

0

Hence,

s = (1/4) [ 2sqrt(5) + ln(2 + sqrt(5)) ]

This is the exact value.

### Exact result

s = (1/4) [ 2sqrt(5) + ln(2 + sqrt(5)) ]

### Approximate value

sqrt(5) ≈ 2.2360679

2sqrt(5) ≈ 4.4721358

ln(2 + sqrt(5)) ≈ ln(4.2360679) ≈ 1.4436355

Add them:

4.4721358 + 1.4436355 = 5.9157713

Now divide by 4:

s ≈ 1.4789428

So,

s ≈ 1.47894

---

## 6. Trapezoidal rule

To approximate

s = ∫_0^1 sqrt(1 + 4t^2) dt

with the trapezoidal rule, divide [0, 1] into N equal parts.

### Step 1. Step size

h = (1 - 0) / N = 1/N

### Step 2. Grid points

t_i = i h, for i = 0, 1, 2, ..., N

### Step 3. Function

f(t) = sqrt(1 + 4t^2)

### Step 4. Trapezoidal approximation

s_N = h [ (1/2)f(t_0) + f(t_1) + f(t_2) + ... + f(t_{N-1}) + (1/2)f(t_N) ]

That is,

s_N = (1/N) [ (1/2)f(0) + Σ_{i=1}^{N-1} f(i/N) + (1/2)f(1) ]

---

## 7. Error

If the exact arc length is s, then the absolute error is

error(N) = |s_N - s|

As N increases, the trapezoidal approximation should converge to the exact value.

---

## 8. Final mathematical results

- r(t) = (t, t^2)
- v(t) = (1, 2t)
- |v(t)| = sqrt(1 + 4t^2)
- s = ∫_0^1 sqrt(1 + 4t^2) dt
- s = (1/4) [ 2sqrt(5) + ln(2 + sqrt(5)) ]
- s ≈ 1.47894

---

HTML/JS app

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Problem 6 - Curve Length and Trapezoidal Rule</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      line-height: 1.4;
      background: #f7f7f7;
      color: #111;
    }
    h1, h2 {
      margin-bottom: 8px;
    }
    .row {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }
    .panel {
      background: white;
      border: 1px solid #ddd;
      border-radius: 10px;
      padding: 16px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.06);
      flex: 1 1 420px;
    }
    canvas {
      border: 1px solid #ccc;
      background: #fff;
      width: 100%;
      max-width: 600px;
      height: 360px;
    }
    label {
      display: inline-block;
      min-width: 180px;
    }
    input[type="range"] {
      width: 280px;
      vertical-align: middle;
    }
    table {
      border-collapse: collapse;
      width: 100%;
      margin-top: 12px;
      font-size: 14px;
    }
    th, td {
      border: 1px solid #ccc;
      padding: 6px 8px;
      text-align: right;
    }
    th {
      background: #f0f0f0;
    }
    .mono {
      font-family: Consolas, monospace;
    }
  </style>
</head>
<body>
  <h1>Problem 6 – Curve Length and Numerical Integration</h1>
  <p>
    Curve:
    <span class="mono">x(t) = t</span>,
    <span class="mono">y(t) = t²</span>,
    <span class="mono">t ∈ [0,1]</span>
  </p>

  <div class="panel">
    <label for="N">Number of trapezoids N:</label>
    <input id="N" type="range" min="2" max="300" step="1" value="20">
    <span id="NValue" class="mono">20</span>
    <button id="recalcBtn">Recalculate</button>

    <p><strong>Velocity vector:</strong> <span class="mono">v(t) = (1, 2t)</span></p>
    <p><strong>Speed:</strong> <span class="mono">|v(t)| = √(1 + 4t²)</span></p>
    <p><strong>Exact arc length:</strong> <span id="exactValue" class="mono"></span></p>
    <p><strong>Trapezoidal approximation:</strong> <span id="trapValue" class="mono"></span></p>
    <p><strong>Absolute error:</strong> <span id="errorValue" class="mono"></span></p>
  </div>

  <div class="row">
    <div class="panel">
      <h2>Trajectory</h2>
      <canvas id="trajCanvas" width="600" height="360"></canvas>
      <p>
        The blue curve is the trajectory. The red points are the trapezoidal partition points used for numerical integration.
      </p>
    </div>

    <div class="panel">
      <h2>Error vs N</h2>
      <canvas id="errorCanvas" width="600" height="360"></canvas>
      <p>
        The graph shows the absolute error <span class="mono">|s_N - s|</span> as the number of divisions N increases.
      </p>
    </div>
  </div>

  <div class="panel">
    <h2>Selected values</h2>
    <table>
      <thead>
        <tr>
          <th>N</th>
          <th>Approximation s_N</th>
          <th>Absolute error</th>
        </tr>
      </thead>
      <tbody id="resultsTable"></tbody>
    </table>
  </div>

  <script>
    function f(t) {
      return Math.sqrt(1 + 4 * t * t);
    }

    function exactArcLength() {
      return 0.25 * (2 * Math.sqrt(5) + Math.log(2 + Math.sqrt(5)));
    }

    function trapezoidalRule(N) {
      const h = 1 / N;
      let sum = 0.5 * f(0) + 0.5 * f(1);
      for (let i = 1; i < N; i++) {
        sum += f(i * h);
      }
      return h * sum;
    }

    function drawAxes(ctx, width, height, margin, xMin, xMax, yMin, yMax) {
      ctx.clearRect(0, 0, width, height);

      ctx.strokeStyle = "#999";
      ctx.lineWidth = 1;

      const x0 = margin;
      const y0 = height - margin;
      const x1 = width - margin;
      const y1 = margin;

      ctx.beginPath();
      ctx.moveTo(x0, y0);
      ctx.lineTo(x1, y0);
      ctx.stroke();

      ctx.beginPath();
      ctx.moveTo(x0, y0);
      ctx.lineTo(x0, y1);
      ctx.stroke();

      ctx.fillStyle = "#111";
      ctx.font = "12px Arial";
      ctx.fillText("x", width - margin + 8, y0 + 4);
      ctx.fillText("y", x0 - 10, margin - 8);
    }

    function mapX(x, width, margin, xMin, xMax) {
      return margin + (x - xMin) * (width - 2 * margin) / (xMax - xMin);
    }

    function mapY(y, height, margin, yMin, yMax) {
      return height - margin - (y - yMin) * (height - 2 * margin) / (yMax - yMin);
    }

    function drawTrajectory(N) {
      const canvas = document.getElementById("trajCanvas");
      const ctx = canvas.getContext("2d");
      const width = canvas.width;
      const height = canvas.height;
      const margin = 40;

      const xMin = 0, xMax = 1;
      const yMin = 0, yMax = 1;

      drawAxes(ctx, width, height, margin, xMin, xMax, yMin, yMax);

      ctx.strokeStyle = "#1565c0";
      ctx.lineWidth = 2;
      ctx.beginPath();

      const M = 400;
      for (let i = 0; i <= M; i++) {
        const t = i / M;
        const x = t;
        const y = t * t;
        const px = mapX(x, width, margin, xMin, xMax);
        const py = mapY(y, height, margin, yMin, yMax);
        if (i === 0) ctx.moveTo(px, py);
        else ctx.lineTo(px, py);
      }
      ctx.stroke();

      ctx.fillStyle = "#c62828";
      for (let i = 0; i <= N; i++) {
        const t = i / N;
        const x = t;
        const y = t * t;
        const px = mapX(x, width, margin, xMin, xMax);
        const py = mapY(y, height, margin, yMin, yMax);
        ctx.beginPath();
        ctx.arc(px, py, 3, 0, 2 * Math.PI);
        ctx.fill();
      }

      ctx.fillStyle = "#111";
      ctx.font = "12px Arial";
      ctx.fillText("(0,0)", mapX(0, width, margin, xMin, xMax) + 4, mapY(0, height, margin, yMin, yMax) - 6);
      ctx.fillText("(1,1)", mapX(1, width, margin, xMin, xMax) - 35, mapY(1, height, margin, yMin, yMax) - 6);
    }

    function drawErrorPlot(currentN) {
      const canvas = document.getElementById("errorCanvas");
      const ctx = canvas.getContext("2d");
      const width = canvas.width;
      const height = canvas.height;
      const margin = 50;

      const exact = exactArcLength();
      const maxN = 300;
      const data = [];
      let maxError = 0;

      for (let N = 2; N <= maxN; N++) {
        const approx = trapezoidalRule(N);
        const err = Math.abs(approx - exact);
        data.push({ N, err });
        if (err > maxError) maxError = err;
      }

      ctx.clearRect(0, 0, width, height);

      ctx.strokeStyle = "#999";
      ctx.lineWidth = 1;

      ctx.beginPath();
      ctx.moveTo(margin, height - margin);
      ctx.lineTo(width - margin, height - margin);
      ctx.stroke();

      ctx.beginPath();
      ctx.moveTo(margin, height - margin);
      ctx.lineTo(margin, margin);
      ctx.stroke();

      ctx.fillStyle = "#111";
      ctx.font = "12px Arial";
      ctx.fillText("N", width - margin + 12, height - margin + 4);
      ctx.fillText("error", margin - 34, margin - 10);

      function px(N) {
        return margin + (N - 2) * (width - 2 * margin) / (maxN - 2);
      }

      function py(err) {
        return height - margin - err * (height - 2 * margin) / maxError;
      }

      ctx.strokeStyle = "#2e7d32";
      ctx.lineWidth = 2;
      ctx.beginPath();

      data.forEach((p, i) => {
        const x = px(p.N);
        const y = py(p.err);
        if (i === 0) ctx.moveTo(x, y);
        else ctx.lineTo(x, y);
      });
      ctx.stroke();

      const currApprox = trapezoidalRule(currentN);
      const currErr = Math.abs(currApprox - exact);

      ctx.fillStyle = "#d32f2f";
      ctx.beginPath();
      ctx.arc(px(currentN), py(currErr), 4, 0, 2 * Math.PI);
      ctx.fill();

      ctx.fillStyle = "#111";
      ctx.fillText(`N = ${currentN}`, px(currentN) + 8, py(currErr) - 8);
    }

    function updateTable() {
      const tbody = document.getElementById("resultsTable");
      const exact = exactArcLength();
      const values = [2, 4, 8, 16, 32, 64, 128, 256];
      tbody.innerHTML = "";

      for (const N of values) {
        const approx = trapezoidalRule(N);
        const err = Math.abs(approx - exact);
        const tr = document.createElement("tr");
        tr.innerHTML = `
          <td>${N}</td>
          <td>${approx.toFixed(10)}</td>
          <td>${err.toExponential(6)}</td>
        `;
        tbody.appendChild(tr);
      }
    }

    function update() {
      const N = parseInt(document.getElementById("N").value, 10);
      document.getElementById("NValue").textContent = N;

      const exact = exactArcLength();
      const approx = trapezoidalRule(N);
      const err = Math.abs(approx - exact);

      document.getElementById("exactValue").textContent = exact.toFixed(10);
      document.getElementById("trapValue").textContent = approx.toFixed(10);
      document.getElementById("errorValue").textContent = err.toExponential(6);

      drawTrajectory(N);
      drawErrorPlot(N);
      updateTable();
    }

    document.getElementById("N").addEventListener("input", update);
    document.getElementById("recalcBtn").addEventListener("click", update);

    update();
  </script>
</body>
</html>
