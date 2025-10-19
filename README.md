<!doctype html>
<html lang="zh-Hant">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>自我介紹 — 你的名字</title>
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#7c3aed; --muted:#94a3b8; --glass: rgba(255,255,255,0.04);
      --radius:16px; --maxw:900px;
    }
    *{box-sizing:border-box}
    body{margin:0; font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, 'Noto Sans TC', 'Microsoft JhengHei', sans-serif; background:linear-gradient(180deg,var(--bg),#071226); color:#e6eef8; display:flex; align-items:center; justify-content:center; min-height:100vh; padding:32px}
    .wrap{width:100%; max-width:var(--maxw); background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); border-radius:20px; padding:28px; box-shadow:0 10px 30px rgba(2,6,23,0.6);}
    header{display:flex; gap:20px; align-items:center}
    .avatar{width:120px; height:120px; border-radius:14px; background:linear-gradient(135deg,var(--accent), #3b82f6); display:flex; align-items:center; justify-content:center; font-weight:700; font-size:40px; color:white}
    h1{margin:0; font-size:26px}
    .subtitle{color:var(--muted); margin-top:6px}
    .grid{display:grid; grid-template-columns:1fr 320px; gap:20px; margin-top:22px}
    .card{background:var(--card); padding:18px; border-radius:var(--radius); box-shadow:0 6px 18px rgba(2,6,23,0.5)}
    .stats{display:flex; gap:12px; margin-top:12px}
    .stat{flex:1; background:var(--glass); padding:12px; border-radius:12px; text-align:center}
    .stat .num{font-weight:700; font-size:20px}
    section h2{margin:0 0 8px 0}
    p{color:#cfe3ff}
    ul{margin:10px 0 0 18px}
    .btn{display:inline-block; padding:10px 14px; border-radius:12px; background:var(--accent); color:white; text-decoration:none; font-weight:600}
    .contact-list{display:flex; flex-direction:column; gap:8px}
    footer{margin-top:18px; color:var(--muted); font-size:13px}
    @media (max-width:860px){
      .grid{grid-template-columns:1fr;}
      .avatar{width:96px;height:96px;font-size:32px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="avatar" aria-hidden="true">

</div>
      <div>
        <h1>麵包</h1>
        <div class="subtitle">嗨！我是 18 歲，身高 189 cm · 熱愛程式與設計</div>
        <div class="stats">
          <div class="stat">
            <div class="num">18</div>
            <div class="muted">年齡</div>
          </div>
          <div class="stat">
            <div class="num">189 cm</div>
            <div class="muted">身高</div>
          </div>
          <div class="stat">
            <div class="num">:D</div>
            <div class="muted">居住桃園 </div>
          </div>
        </div>
      </div>
    </header>

    <div class="grid">
      <main>
        <div class="card">
          <section>
            <h2>關於我</h2>
            <p>我是大學新鮮人，喜歡學習前端、遊戲開發與視覺設計。平時會用 HTML/CSS/JavaScript 製作小專案，對創意,我好無聊 快找我打遊戲:D</p>
          </section>

          <section style="margin-top:14px">
            <h2>技能</h2>
            <ul>
              <li>HTML & CSS（含 RWD）</li>
              <li>JavaScript 基礎互動</li>
              <li>簡易圖像/影像處理（Photoshop / Figma）</li>
              <li>會用 Git 版本控制（或填寫你的技能）</li>
            </ul>
          </section>

          <section style="margin-top:14px">
            <h2>作品/興趣</h2>
            <p>可以把你做過的小遊戲、網站或其他作品放在這裡（連結、圖片或簡短說明）。</p>
            <p style="margin-top:6px"><a class="btn" href="#projects">目前沒有作品</a></p>
          </section>
        </div>

        <div class="card" id="projects" style="margin-top:14px">
          <h2>小專案</h2>
          <ul>
            <li>個人首頁 — 使用純 HTML/CSS 建構</li>
            <li>互動小遊戲 — 簡單的 2D 射擊或計分遊戲</li>
            <li>動畫履歷 — 利用 CSS 動畫呈現經歷</li>
          </ul>
        </div>

        <footer>
          <div>提示：打開本檔案後把「你的名字」替換成真實名字，將 avatar 的文字改成你的姓名首字或上傳一張照片（替換 .avatar 的背景）。</div>
        </footer>
      </main>

      <aside>
        <div class="card">
          <h2>聯絡方式</h2>
          <div class="contact-list">
            <div>Email: <a href="mailto:a0968570946@gmail.com">a0968570946@gmail.com</a></div>
            <div>Phone: +886 0968570946 </div>
            <div>IG: @_3wellr.0211</div>
          </div>

          <div style="margin-top:14px">
            <a class="btn" href="mailto:example@example.com?subject=聯絡%20自我介紹">歡迎聯絡我</a>
          </div>
        </div>

        <div class="card" style="margin-top:14px">
          <h2>個性標籤</h2>
          <p>好聊天 · 細心 · 樂於合作 . 外向 .愛騎車 </p>
        </div>

        <div class="card" style="margin-top:14px; text-align:center">
              </div>
      </aside>
    </div>
  </div>

  <script>
    // 簡單互動：按下 avatar 可在頁面上顯示提示（示範用途）
    document.querySelector('.avatar').addEventListener('click', ()=>{
      alert('把這裡替換成你的照片或姓名縮寫！');
    });
  </script>
</body>
</h
