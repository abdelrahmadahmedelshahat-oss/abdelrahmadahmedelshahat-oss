<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Abdelrahman Ahmed Elshahat — GitHub Profile</title>
<style>
  * { box-sizing: border-box; }
  body {
    margin: 0;
    background: #0d1117;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
    color: #c9d1d9;
    line-height: 1.6;
  }
  .wrapper {
    max-width: 920px;
    margin: 0 auto;
    padding: 32px 16px;
  }
  .hero {
    text-align: center;
    margin-bottom: 24px;
  }
  .hero img { border-radius: 8px; }
  .hero h1 { margin: 12px 0 4px; font-size: 28px; }
  .hero p { margin: 0; color: #8b949e; font-size: 16px; }

  details {
    background: #161b22;
    border: 1px solid #30363d;
    border-radius: 10px;
    padding: 12px 16px;
    margin-bottom: 16px;
  }
  summary {
    font-weight: 600;
    cursor: pointer;
    color: #58a6ff;
  }
  details p { margin: 8px 0 0; color: #8b949e; }

  .badges-row {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    justify-content: center;
    margin-bottom: 16px;
  }
  .badge-img { height: 20px; border-radius: 4px; }

  pre {
    background: #161b22;
    border: 1px solid #30363d;
    border-radius: 10px;
    padding: 16px;
    overflow-x: auto;
    font-size: 13px;
    color: #c9d1d9;
    margin-bottom: 24px;
  }
  code { font-family: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, monospace; }
  .keyword { color: #ff7b72; }
  .type { color: #79c0ff; }
  .string { color: #a5d6ff; }
  .func { color: #d2a8ff; }
  .comment { color: #8b949e; }

  /* ===== Interactive Widget ===== */
  .gh-profile {
    --bg: #0d1117;
    --card-bg: #161b22;
    --border: #30363d;
    --text: #c9d1d9;
    --text-secondary: #8b949e;
    --accent: #58a6ff;
    --cpp: #f34b7d;
    background: var(--bg);
    color: var(--text);
    padding: 24px;
    border-radius: 12px;
    border: 1px solid var(--border);
    position: relative;
  }
  .gh-header {
    display: flex;
    align-items: flex-start;
    gap: 16px;
    margin-bottom: 20px;
  }
  .gh-avatar {
    width: 64px; height: 64px;
    border-radius: 50%;
    border: 2px solid var(--border);
  }
  .gh-info h2 { margin: 0 0 4px 0; font-size: 20px; }
  .gh-info p { margin: 0; color: var(--text-secondary); font-size: 14px; }
  .gh-badges {
    display: flex; flex-wrap: wrap; gap: 6px; margin: 12px 0;
  }
  .gh-badge {
    display: inline-flex; align-items: center; gap: 4px;
    padding: 4px 10px; border-radius: 20px;
    font-size: 12px; font-weight: 600;
    border: 1px solid var(--border); background: var(--card-bg);
  }
  .gh-list { list-style: none; padding: 0; margin: 0 0 20px 0; }
  .gh-list li {
    display: flex; align-items: center; gap: 10px;
    padding: 6px 0; font-size: 14px; color: var(--text-secondary);
  }
  .gh-list li span { font-size: 16px; }
  .gh-stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 12px; margin-bottom: 16px;
  }
  .gh-stat-card {
    background: var(--card-bg); border: 1px solid var(--border);
    border-radius: 10px; padding: 16px;
    transition: transform 0.2s, border-color 0.2s;
  }
  .gh-stat-card:hover {
    transform: translateY(-2px); border-color: var(--accent);
  }
  .gh-stat-card h3 { margin: 0 0 12px 0; font-size: 14px; font-weight: 600; }
  .gh-chart-wrap {
    display: flex; align-items: center; justify-content: center;
    gap: 16px; flex-wrap: wrap;
  }
  .gh-donut { width: 120px; height: 120px; }
  .gh-legend { display: flex; flex-direction: column; gap: 6px; font-size: 12px; }
  .gh-legend-item { display: flex; align-items: center; gap: 6px; color: var(--text-secondary); }
  .gh-dot { width: 10px; height: 10px; border-radius: 2px; }
  .gh-more {
    text-align: center; margin: 12px 0; font-size: 13px;
    color: var(--text-secondary); cursor: pointer; user-select: none;
  }
  .gh-more:hover { color: var(--accent); }
  .gh-cycle { text-align: center; margin-top: 20px; padding-top: 16px; border-top: 1px solid var(--border); }
  .gh-cycle h4 { margin: 0 0 12px 0; font-size: 14px; color: var(--text-secondary); font-weight: 400; }
  .gh-emojis { display: flex; justify-content: center; gap: 24px; font-size: 40px; }
  .gh-emoji { animation: bounce 2s infinite; cursor: pointer; transition: transform 0.2s; }
  .gh-emoji:hover { transform: scale(1.2); }
  .gh-emoji:nth-child(2) { animation-delay: 0.3s; }
  .gh-emoji:nth-child(3) { animation-delay: 0.6s; }
  @keyframes bounce { 0%,100%{transform:translateY(0);} 50%{transform:translateY(-8px);} }
  .gh-penguin {
    position: absolute; top: 24px; right: 24px; width: 80px;
    animation: waddle 3s ease-in-out infinite;
  }
  @keyframes waddle { 0%,100%{transform:rotate(-3deg);} 50%{transform:rotate(3deg);} }
  .gh-track { fill:none; stroke:#30363d; stroke-width:3; }
  .gh-cpp-full { fill:none; stroke:var(--cpp); stroke-width:3; stroke-dasharray:100,0; }
</style>
<base target="_blank">
</head>
<body>
<div class="wrapper">

  <!-- Hero -->
  <div class="hero">
    <img src="https://cdn.dribbble.com/users/1162077/screenshots/3848914/programmer.gif" alt="Hacker Boy Coding" width="60%"/><br>
    <img src="https://user-images.githubusercontent.com/74038190/221352989-518609ab-b4d1-459e-929f-a08cd2bd9b3c.gif" alt="Cybersecurity" width="40%"/><br>
    <h1>Hi, I'm Abdelrahman Ahmed Elshahat 👋</h1>
    <p><strong>Cybersecurity Learner | C++ & Data Structures | Linux Enthusiast</strong></p>
  </div>

  <!-- Details -->
  <details>
    <summary><strong>Currently learning & building :</strong></summary>
    <p>🔐 On my way to becoming a Cybersecurity Analyst — building the fundamentals first, the right way.</p>
  </details>

  <!-- Badges -->
  <div class="badges-row">
    <img class="badge-img" src="https://komarev.com/ghpvc/?username=abdelrahmanahmedelshahat-oss&style=flat&color=orange&label=PROFILE+VIEWS" alt="Profile Views">
    <img class="badge-img" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fabdelrahmanahmedelshahat-oss&count_bg=%2379C83D&title_bg=%23555555&icon=mediafire.svg&icon_color=%23E7E7E7&title=HITS&edge_flat=false" alt="Hits">
    <img class="badge-img" src="https://img.shields.io/badge/Contact-Telegram-grey?style=flat&logo=telegram" alt="Telegram">
  </div>

  <!-- Tools -->
  <div class="badges-row">
    <img class="badge-img" src="https://img.shields.io/badge/-%F0%9F%9A%80%20Tools%20I%20use-orange" alt="Tools">
    <img class="badge-img" src="https://img.shields.io/badge/-%3A-orange" alt="semicolon">
    <img class="badge-img" src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=c%2B%2B&logoColor=white" alt="C++">
    <img class="badge-img" src="https://img.shields.io/badge/OOP-3776AB?style=flat&logo=cplusplus&logoColor=white" alt="OOP">
    <img class="badge-img" src="https://img.shields.io/badge/Data_Structures-FF6F00?style=flat&logo=unrealengine&logoColor=white" alt="Data Structures">
    <img class="badge-img" src="https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black" alt="Linux">
    <img class="badge-img" src="https://img.shields.io/badge/GNU%20Bash-4EAA25?style=flat&logo=GNU%20Bash&logoColor=white" alt="Bash">
    <img class="badge-img" src="https://img.shields.io/badge/GIT-E44C30?style=flat&logo=git&logoColor=white" alt="Git">
    <img class="badge-img" src="https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=flat&logo=visual%20studio%20code&logoColor=white" alt="VS Code">
    <img class="badge-img" src="https://img.shields.io/badge/TryHackMe-212C42?style=flat&logo=tryhackme&logoColor=red" alt="TryHackMe">
  </div>

  <!-- C++ Code Block -->
  <pre><code><span class="comment">// about_me.cpp</span>

<span class="keyword">#include</span> <span class="string">&lt;iostream&gt;</span>
<span class="keyword">#include</span> <span class="string">&lt;vector&gt;</span>
<span class="keyword">#include</span> <span class="string">&lt;string&gt;</span>

<span class="keyword">class</span> <span class="type">Me</span> {
<span class="keyword">private</span>:
    std::string name = <span class="string">"Abdelrahman Ahmed Elshahat"</span>;
    std::vector&lt;std::string&gt; currentSkills = {
        <span class="string">"C++"</span>, <span class="string">"OOP"</span>, <span class="string">"Data Structures"</span>, <span class="string">"Linux Basics"</span>
    };
    std::vector&lt;std::string&gt; learningPath = {
        <span class="string">"Networking"</span>, <span class="string">"Linux (Advanced)"</span>, <span class="string">"SQL Basics"</span>,
        <span class="string">"Cybersecurity Fundamentals"</span>, <span class="string">"TryHackMe"</span>
    };
    std::string goal = <span class="string">"Cybersecurity Analyst"</span>;

<span class="keyword">public</span>:
    <span class="type">void</span> <span class="func">introduce</span>() {
        std::cout &lt;&lt; <span class="string">"Hi, I'm "</span> &lt;&lt; name &lt;&lt; std::endl;
        std::cout &lt;&lt; <span class="string">"Currently mastering the fundamentals,"</span> &lt;&lt; std::endl;
        std::cout &lt;&lt; <span class="string">"one Data Structure at a time."</span> &lt;&lt; std::endl;
        std::cout &lt;&lt; <span class="string">"Goal: "</span> &lt;&lt; goal &lt;&lt; <span class="string">" 🔐"</span> &lt;&lt; std::endl;
    }
};

<span class="type">int</span> <span class="func">main</span>() {
    Me abdelrahman;
    abdelrahman.introduce();
    <span class="keyword">return</span> 0;
}</code></pre>

  <hr style="border:0;border-top:1px solid #30363d;margin:24px 0;">

  <!-- ===== Interactive Widget ===== -->
  <div class="gh-profile">
    <img class="gh-penguin" src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Animals/Penguin.png" alt="penguin">

    <div class="gh-header">
      <img class="gh-avatar" src="https://avatars.githubusercontent.com/u/0?v=4" alt="avatar">
      <div class="gh-info">
        <h2>Abdelrahman Ahmed Elshahat</h2>
        <p>Cybersecurity Learner | C++ & Data Structures | Linux Enthusiast</p>
        <div class="gh-badges">
          <span class="gh-badge" style="color:#58a6ff">🔐 Security</span>
          <span class="gh-badge" style="color:#f34b7d">C++</span>
          <span class="gh-badge" style="color:#FCC624">🐧 Linux</span>
        </div>
      </div>
    </div>

    <ul class="gh-list">
      <li><span>🎓</span> I'm currently learning Frappe.</li>
      <li><span>🐧</span> I like exploring GNU/Linux.</li>
      <li><span>💬</span> Ask me about PC building, Movies, or anything.</li>
      <li><span>📬</span> Find me on Telegram: <a href="https://t.me/abdelrahmanahmedelshahat" style="color:var(--accent);text-decoration:none;">@abdelrahmanahmedelshahat</a></li>
      <li><span>⚡</span> Fun fact: Banging your head against a wall for one hour burns 150 calories.</li>
    </ul>

    <div class="gh-stats-grid">
      <div class="gh-stat-card">
        <h3>📊 Top Languages by Repo</h3>
        <div class="gh-chart-wrap">
          <svg class="gh-donut" viewBox="0 0 36 36">
            <path class="gh-track" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
            <path class="gh-cpp-full" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
          </svg>
          <div class="gh-legend">
            <div class="gh-legend-item"><div class="gh-dot" style="background:#f34b7d"></div> C++</div>
          </div>
        </div>
      </div>

      <div class="gh-stat-card">
        <h3>🔥 Top Languages by Commit</h3>
        <div class="gh-chart-wrap">
          <svg class="gh-donut" viewBox="0 0 36 36">
            <path class="gh-track" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
            <path class="gh-cpp-full" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
          </svg>
          <div class="gh-legend">
            <div class="gh-legend-item"><div class="gh-dot" style="background:#f34b7d"></div> C++</div>
          </div>
        </div>
      </div>
    </div>

    <div class="gh-more" onclick="this.nextElementSibling.style.display=this.nextElementSibling.style.display==='none'?'block':'none'">
      ▶ More stats
    </div>
    <div style="display:none;background:var(--card-bg);border:1px solid var(--border);border-radius:10px;padding:16px;margin-top:8px;">
      <div style="display:flex;justify-content:space-between;padding:4px 0;font-size:13px;color:var(--text-secondary);"><span>Longest streak:</span> <strong style="color:var(--text);">42 days</strong></div>
      <div style="display:flex;justify-content:space-between;padding:4px 0;font-size:13px;color:var(--text-secondary);"><span>Current streak:</span> <strong style="color:var(--text);">7 days</strong></div>
      <div style="display:flex;justify-content:space-between;padding:4px 0;font-size:13px;color:var(--text-secondary);"><span>Total repositories:</span> <strong style="color:var(--text);">24</strong></div>
    </div>

    <div class="gh-cycle">
      <h4>Code Cycle</h4>
      <div class="gh-emojis">
        <div class="gh-emoji" title="Debugging">😵‍💫</div>
        <div class="gh-emoji" title="It works!">😌</div>
        <div class="gh-emoji" title="Wait, what?">🤪</div>
      </div>
    </div>
  </div>

</div>
</body>
</html>
