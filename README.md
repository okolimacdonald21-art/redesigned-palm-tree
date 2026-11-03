# redesigned-palm-tree
All over the world can make use of it
<!doctype html>

<html lang="en">  
<head>  
  <meta charset="utf-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1">  
  <meta name="description" content="Independent assistance preparing military-family leave inquiries.">  
  <title>Leave Request Support</title>    <style>  
    :root {  
      --navy: #14283f;  
      --blue: #245b82;  
      --gold: #d7a94b;  
      --ink: #1d2935;  
      --muted: #647384;  
      --paper: #fff;  
      --background: #f3f6f8;  
      --line: #dce4ea;  
      --warning-bg: #fff8e9;  
      --warning-border: #e6bd63;  
      --radius: 16px;  
      --shadow: 0 14px 40px rgba(20, 40, 63, .08);  
    }  
  
    * { box-sizing: border-box; }  
  
    html { scroll-behavior: smooth; }  
  
    body {  
      margin: 0;  
      color: var(--ink);  
      background: var(--background);  
      font: 16px/1.6 system-ui, -apple-system, "Segoe UI", sans-serif;  
    }  
  
    a { color: var(--blue); }  
  
    .container {  
      width: min(1120px, calc(100% - 40px));  
      margin-inline: auto;  
    }  
  
    .top-note {  
      padding: 10px 20px;  
      color: #fff;  
      background: var(--navy);  
      text-align: center;  
      font-size: .9rem;  
    }  
  
    header {  
      background: var(--paper);  
      border-bottom: 1px solid var(--line);  
    }  
  
    .nav {  
      min-height: 76px;  
      display: flex;  
      align-items: center;  
      justify-content: space-between;  
      gap: 24px;  
    }  
  
    .brand {  
      display: flex;  
      align-items: center;  
      gap: 12px;  
      color: var(--navy);  
      font-weight: 750;  
      text-decoration: none;  
    }  
  
    .brand-mark {  
      display: grid;  
      width: 42px;  
      height: 42px;  
      place-items: center;  
      border-radius: 12px;  
      color: var(--navy);  
      background: #f4e8c9;  
      font-size: 1.25rem;  
    }  
  
    nav { display: flex; gap: 22px; flex-wrap: wrap; }  
    nav a { color: var(--ink); text-decoration: none; font-weight: 600; }  
    nav a:hover { color: var(--blue); }  
  
    .hero {  
      padding: 76px 0 58px;  
      background:  
        radial-gradient(circle at 85% 20%, rgba(215,169,75,.16), transparent 28%),  
        linear-gradient(135deg, #edf3f7, #fff);  
    }  
  
    .hero-grid {  
      display: grid;  
      grid-template-columns: 1.25fr .75fr;  
      gap: 48px;  
      align-items: center;  
    }  
  
    .eyebrow {  
      color: var(--blue);  
      text-transform: uppercase;  
      letter-spacing: .12em;  
      font-size: .78rem;  
      font-weight: 800;  
    }  
  
    h1, h2, h3 { color: var(--navy); line-height: 1.2; }  
    h1 { max-width: 720px; margin: 12px 0 18px; font-size: clamp(2.4rem, 5vw, 4.2rem); }  
    h2 { margin: 0 0 14px; font-size: clamp(1.8rem, 3vw, 2.5rem); }  
    h3 { margin-top: 0; }  
  
    .lead { max-width: 680px; color: var(--muted); font-size: 1.12rem; }  
  
    .button {  
      display: inline-flex;  
      justify-content: center;  
      align-items: center;  
      min-height: 48px;  
      padding: 12px 20px;  
      border: 0;  
      border-radius: 10px;  
      background: var(--navy);  
      color: #fff;  
      font: inherit;  
      font-weight: 750;  
      text-decoration: none;  
      cursor: pointer;  
    }  
  
    .button:hover { background: var(--blue); }  
  
    .button-outline {  
      color: var(--navy);  
      background: transparent;  
      border: 1px solid #aebdca;  
    }  
  
    .button-outline:hover { color: #fff; }  
  
    .actions { display: flex; gap: 12px; flex-wrap: wrap; margin-top: 26px; }  
  
    .notice {  
      padding: 18px 20px;  
      border: 1px solid var(--warning-border);  
      border-left: 5px solid var(--gold);  
      border-radius: 12px;  
      background: var(--warning-bg);  
      color: #59451a;  
    }  
  
    .notice strong { display: block; margin-bottom: 4px; }  
  
    .hero-card, .panel, .step {  
      background: var(--paper);  
      border: 1px solid var(--line);  
      border-radius: var(--radius);  
      box-shadow: var(--shadow);  
    }  
  
    .hero-card { padding: 26px; }  
    .hero-card ul { margin-bottom: 0; padding-left: 20px; color: var(--muted); }  
    .hero-card li { margin: 8px 0; }  
  
    section { padding: 64px 0; }  
    .section-intro { max-width: 690px; margin-bottom: 28px; color: var(--muted); }  
  
    .steps {  
      display: grid;  
      grid-template-columns: repeat(3, 1fr);  
      gap: 18px;  
    }  
  
    .step { padding: 22px; box-shadow: none; }  
    .step-number {  
      display: grid;  
      width: 36px;  
      height: 36px;  
      place-items: center;  
      margin-bottom: 16px;  
      border-radius: 50%;  
      background: #f4e8c9;  
      color: var(--navy);  
      font-weight: 800;  
    }  
  
    .step p { margin-bottom: 0; color: var(--muted); }  
  
    .form-section { background: #eaf0f4; }  
    .panel { padding: clamp(20px, 4vw, 38px); }  
  
    form { display: grid; gap: 18px; }  
    .form-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; }  
  
    label, legend { display: block; margin-bottom: 7px; color: var(--navy); font-weight: 700; }  
  
    input, select, textarea {  
      width: 100%;  
      min-height: 48px;  
      padding: 12px 13px;  
      border: 1px solid #c8d3dc;  
      border-radius: 9px;  
      background: #fff;  
      color: var(--ink);  
      font: inherit;  
    }  
  
    textarea { min-height: 130px; resize: vertical; }  
    input:focus, select:focus, textarea:focus { outline: 3px solid #b9d5e8; border-color: var(--blue); }  
  
    .help, .privacy-copy { color: var(--muted); font-size: .9rem; }  
    .check-row { display: flex; align-items: flex-start; gap: 10px; }  
    .check-row input { width: 18px; min-height: 18px; margin-top: 4px; }  
    .check-row label { margin: 0; font-weight: 500; }  
  
    .contact-card {  
      display: flex;  
      justify-content: space-between;  
      align-items: center;  
      gap: 24px;  
      padding: 28px;  
      border-radius: var(--radius);  
      background: var(--navy);  
      color: #fff;  
    }  
  
    .contact-card h2 { color: #fff; }  
    .contact-card p { margin-bottom: 0; color: #d7e1e9; }  
    .contact-card a { color: #fff; font-weight: 700; }  
  
    footer { padding: 26px 0; background: #0e1e30; color: #d7e1e9; font-size: .9rem; }  
    footer p { margin: 6px 0; }  
  
    @media (max-width: 760px) {  
      .nav { align-items: flex-start; flex-direction: column; padding: 16px 0; }  
      nav { gap: 14px; }  
      .hero-grid, .steps, .form-grid { grid-template-columns: 1fr; }  
      .hero { padding-top: 50px; }  
      .contact-card { align-items: flex-start; flex-direction: column; }  
    }  
  </style>  </head>  <body>  
  <div class="top-note">  
    Independent private service · Not a military or government agency  
  </div>    <header>  
    <div class="container nav">  
      <a class="brand" href="#home">  
        <span class="brand-mark" aria-hidden="true">LS</span>  
        <span>Leave Request Support</span>  
      </a>  
      <nav aria-label="Main navigation">  
        <a href="#how-it-works">How it works</a>  
        <a href="#request">Request assistance</a>  
        <a href="#contact">Contact</a>  
      </nav>  
    </div>  
  </header>    <main>  
    <section class="hero" id="home">  
      <div class="container hero-grid">  
        <div>  
          <div class="eyebrow">Independent request-preparation assistance</div>  
          <h1>Help organizing a leave request</h1>  
          <p class="lead">  
            We help clients prepare and organize information for a leave-related inquiry.  
            We do not issue leave permits, contact a military unit on your behalf, or decide  
            whether a request will be approved.  
          </p>  
          <div class="actions">  
            <a class="button" href="#request">Request assistance</a>  
            <a class="button button-outline" href="#how-it-works">Learn how it works</a>  
          </div>  
        </div>  <aside class="hero-card">  
      <h3>Before you submit</h3>  
      <div class="notice">  
        <strong>Important</strong>  
        This is a private, independent service. It is not affiliated with or endorsed by  
        any military branch or government agency. Only the appropriate official authority  
        can approve leave.  
      </div>  
      <ul>  
        <li>Submitting this form does not create an official leave application.</li>  
        <li>We cannot guarantee approval or a specific decision.</li>  
        <li>For urgent matters, contact the appropriate official channel directly.</li>  
      </ul>  
    </aside>  
  </div>  
</section>  

<section id="how-it-works">  
  <div class="container">  
    <div class="eyebrow">The process</div>  
    <h2>How it works</h2>  
    <p class="section-intro">  
      Send us the basic details about the assistance you need. We’ll contact you using  
      the email address you provide to discuss next steps.  
    </p>  

    <div class="steps">  
      <article class="step">  
        <div class="step-number">1</div>  
        <h3>Send an inquiry</h3>  
        <p>Choose a request category and share only the information needed to explain your inquiry.</p>  
      </article>  
      <article class="step">  
        <div class="step-number">2</div>  
        <h3>We review it</h3>  
        <p>Our private service reviews the inquiry and contacts you. Any fees and service limits should be disclosed before work begins.</p>  
      </article>  
      <article class="step">  
        <div class="step-number">3</div>  
        <h3>Use official channels</h3>  
        <p>Any actual leave decision must come from the appropriate military authority through its official process.</p>  
      </article>  
    </div>  
  </div>  
</section>  

<section class="form-section" id="request">  
  <div class="container">  
    <div class="eyebrow">Get in touch</div>  
    <h2>Request assistance</h2>  
    <p class="section-intro">  
      This form sends an inquiry to the private service operator, not to a military authority.  
    </p>  

    <div class="panel">  
      <!-- Replace the action URL with your verified form-provider endpoint. -->  
      <form action="https://formspree.io/f/REPLACE_WITH_YOUR_FORM_ID" method="POST">  
        <div class="form-grid">  
          <div>  
            <label for="client-name">Your full name</label>  
            <input id="client-name" name="client_name" autocomplete="name" required>  
          </div>  
          <div>  
            <label for="client-email">Your email address</label>  
            <input id="client-email" name="email" type="email" autocomplete="email" required>  
          </div>  
        </div>  

        <div class="form-grid">  
          <div>  
            <label for="service-member">Service member’s name</label>  
            <input id="service-member" name="service_member_name">  
            <div class="help">Do not include rank, unit, duty location, or other sensitive details.</div>  
          </div>  
          <div>  
            <label for="relationship">Your relationship</label>  
            <input id="relationship" name="relationship" placeholder="For example: fiancé, spouse, or family member">  
          </div>  
        </div>  

        <div>  
          <label for="request-type">Type of assistance requested</label>  
          <select id="request-type" name="request_type" required>  
            <option value="">Select a category</option>  
            <option>3-month leave-related inquiry</option>  
            <option>6-month leave-related inquiry</option>  
            <option>Retirement-related inquiry</option>  
            <option>Other leave-related inquiry</option>  
          </select>  
          <div class="help">These are inquiry categories, not available leave entitlements or permits.</div>  
        </div>  

        <div class="form-grid">  
          <div>  
            <label for="origin">Country or region you are from</label>  
            <input id="origin" name="origin" autocomplete="country-name">  
          </div>  
          <div>  
            <label for="current-location">Country or region where you currently live</label>  
            <input id="current-location" name="current_location" autocomplete="country-name">  
          </div>  
        </div>  

        <div>  
          <label for="reason">Reason for your inquiry</label>  
          <textarea id="reason" name="reason" required  
            placeholder="Briefly explain what help you are looking for. Do not include passwords, financial details, or sensitive medical or military information."></textarea>  
        </div>  

        <div class="check-row">  
          <input id="acknowledgment" name="acknowledgment" type="checkbox" required>  
          <label for="acknowledgment">  
            I understand this is a private service, not an official military or government service,  
            and submitting this form does not apply for or guarantee approved leave.  
          </label>  
        </div>  

        <p class="privacy-copy">  
          By submitting, you are asking the private service operator to contact you about your inquiry.  
          Add a full privacy notice explaining how information is stored, who can access it, how long  
          it is kept, and how to request deletion before publishing this form.  
        </p>  

        <button class="button" type="submit">Send inquiry</button>  
      </form>  
    </div>  
  </div>  
</section>  

<section id="contact">  
  <div class="container">  
    <div class="contact-card">  
      <div>  
        <div class="eyebrow" style="color:#e8c875">Contact</div>  
        <h2>Questions before submitting?</h2>  
        <p>Contact the private service operator using the email below.</p>  
      </div>  
      <a href="mailto:YOUR_EMAIL@example.com">YOUR_EMAIL@example.com</a>  
    </div>  
  </div>  
</section>

  </main>    <footer>  
    <div class="container">  
      <p><strong>Leave Request Support</strong> is an independent private service.</p>  
      <p>Not affiliated with or endorsed by any military branch or government agency. No leave approval or permit is issued by this website.</p>  
      <p>© 2026 Leave Request Support</p>  
    </div>  
  </footer>  
</body>  
</html>  Create a website with this code
