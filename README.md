<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Family Shirt Clip Animation</title>
  <style>
    body {
      background: #f4f8fb;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .scene {
      width: 400px;
      height: 300px;
      position: relative;
      background: #e4e8ee;
      border-radius: 20px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.12);
    }
    .sofa {
      position: absolute;
      bottom: 40px;
      left: 40px;
      width: 320px;
      height: 80px;
      background: #b2b7c7;
      border-radius: 40px 40px 20px 20px;
    }
    .person {
      position: absolute;
      width: 60px;
      height: 100px;
      animation: bounce 1s infinite alternate;
    }
    .parent1 { left: 60px; bottom: 90px; }
    .parent2 { left: 180px; bottom: 90px; }
    .grandchild { left: 120px; bottom: 70px; animation: jump 1s infinite alternate; }

    @keyframes bounce {
      to { transform: translateY(-10px); }
    }
    @keyframes jump {
      to { transform: translateY(-30px); }
    }
  </style>
</head>
<body>
  <div class="scene">
    <div class="sofa"></div>
    <!-- Parent 1 -->
    <svg class="person parent1" viewBox="0 0 60 100">
      <ellipse cx="30" cy="22" rx="18" ry="20" fill="#f7d6b3"/>
      <rect x="18" y="40" width="24" height="40" rx="12" fill="#5a6ca1"/>
      <rect x="18" y="80" width="10" height="20" rx="5" fill="#f7d6b3"/>
      <rect x="32" y="80" width="10" height="20" rx="5" fill="#f7d6b3"/>
    </svg>
    <!-- Parent 2 -->
    <svg class="person parent2" viewBox="0 0 60 100">
      <ellipse cx="30" cy="22" rx="18" ry="20" fill="#f3c3aa"/>
      <rect x="18" y="40" width="24" height="40" rx="12" fill="#b1cc8a"/>
      <rect x="18" y="80" width="10" height="20" rx="5" fill="#f3c3aa"/>
      <rect x="32" y="80" width="10" height="20" rx="5" fill="#f3c3aa"/>
    </svg>
    <!-- Grandchild -->
    <svg class="person grandchild" viewBox="0 0 60 100">
      <ellipse cx="30" cy="22" rx="16" ry="18" fill="#efb2a8"/>
      <rect x="20" y="40" width="20" height="38" rx="10" fill="#f7e04b"/>
      <rect x="20" y="78" width="8" height="18" rx="4" fill="#efb2a8"/>
      <rect x="32" y="78" width="8" height="18" rx="4" fill="#efb2a8"/>
    </svg>
  </div>
</body>
</html>