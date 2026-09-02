---
title: Home
---
<style>
:root {
  --bg: #0b0b0f;
  --card: #14141a;
  --card2: #1a1a22;
  --text: #f7f7fb;
  --muted: #a8a8b5;
  --line: #2a2a34;
  --accent: #ff4f8b;
  --accent2: #8b5cf6;
  --max: 920px;
}
* { box-sizing: border-box; }
html { scroll-behavior: smooth; }
body {
  margin: 0;
  background:
    radial-gradient(circle at 15% 0%, rgba(255,79,139,.16), transparent 32rem),
    radial-gradient(circle at 85% 5%, rgba(139,92,246,.15), transparent 30rem),
    var(--bg);
  color: var(--text);
  font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont,
               "Segoe UI", sans-serif;
  line-height: 1.7;
}
.wrap { width: min(calc(100% - 40px), var(--max)); margin: 0 auto; }
.hero { padding: 72px 0 44px; }
.badge {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 7px 12px;
  border: 1px solid var(--line);
  border-radius: 999px;
  background: rgba(255,255,255,.045);
  color: #dddde7;
  font-size: 13px;
  font-weight: 650;
  letter-spacing: .02em;
}
h1 {
  margin: 18px 0 10px;
  font-size: clamp(38px, 7vw, 64px);
  line-height: 1.03;
  letter-spacing: -.045em;
}
.subtitle {
  margin: 0;
  max-width: 680px;
  color: var(--muted);
  font-size: 18px;
}
.updated { margin-top: 18px; color: #777784; font-size: 14px; }
main { padding-bottom: 70px; }
.card {
  margin: 18px 0;
  padding: 30px;
  background: rgba(20,20,26,.88);
  border: 1px solid var(--line);
  border-radius: 22px;
  box-shadow: 0 16px 50px rgba(0,0,0,.22);
}
h2 {
  margin: 0 0 14px;
  font-size: 25px;
  line-height: 1.2;
  letter-spacing: -.02em;
}
p { margin: 10px 0; }
a { color: #ff8db3; text-decoration: none; }
a:hover { text-decoration: underline; }
strong { color: #fff; }
ul, ol { padding-left: 22px; }
li { margin: 8px 0; color: #c9c9d3; }
.callout {
  padding: 18px 20px;
  border-left: 3px solid var(--accent);
  background: rgba(255,79,139,.06);
  border-radius: 0 14px 14px 0;
  color: #d9d9e2;
  margin-top: 18px;
}
.footer {
  padding: 30px 0 50px;
  color: #777784;
  text-align: center;
  font-size: 13px;
}
@media (max-width: 640px) {
  .wrap { width: min(calc(100% - 24px), var(--max)); }
  .hero { padding: 46px 0 28px; }
  .card { padding: 22px 18px; border-radius: 18px; }
  h2 { font-size: 22px; }
}
</style>

<header class="hero">
  <div class="wrap">
    <span class="badge">Wecide · com.wecide.app</span>
    <h1>Wecide</h1>
    <p class="subtitle">
      Wecide helps a group of people pick a film to watch together.
      The application is built entirely around privacy and frictionless use: there is no sign-up, no email address, and no password required.
    </p>
  </div>
</header>

<main class="wrap">

<section class="card">
  <h2>How It Works</h2>
  <ol>
    <li><strong>Start a Room:</strong> An anonymous identifier is created automatically to tell your device apart from others.</li>
    <li><strong>Invite Friends:</strong> Users join a shared session using a room code.</li>
    <li><strong>Set the Vibe:</strong> The room's settings (streaming services, moods, eras, and session length) determine which films appear in the deck.</li>
    <li><strong>Vote:</strong> Submit your vote on each film using a like, pass, or super like.</li>
    <li><strong>Decide:</strong> Wecide detects when everyone agrees and builds the final results screen.</li>
  </ol>
</section>

<section class="card">
  <h2>Privacy & Data</h2>
  <p>Wecide is completely ad-free and contains no analytics tracking or crash-reporting software.</p>
  <ul>
    <li><strong>No Accounts:</strong> You are never asked for an email, phone number, or password.</li>
    <li><strong>Ephemeral Data:</strong> A room and everything in it (members, votes, settings) is deleted automatically <strong>24 hours</strong> after creation.</li>
    <li><strong>Third-Party Providers:</strong> We use <strong>Supabase</strong> for secure, anonymous database hosting and <strong>TMDB</strong> for film information and posters. Your votes and identifiers are never sent to TMDB.</li>
  </ul>
  <div class="callout">
    For full details, please review our <a href="wecide-privacy-policy.html">Privacy Policy</a>.
  </div>
</section>

<section class="card">
  <h2>Contact</h2>
  <p>Wecide is published and operated by Carolina Campos. If you have questions about the app or data handling, reach out at <a href="mailto:gr.camposr@gmail.com">gr.camposr@gmail.com</a>.</p>
</section>

</main>
