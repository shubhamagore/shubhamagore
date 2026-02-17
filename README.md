<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Shubham Gore – GitHub Profile README</title>
    <link
      href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;600&display=swap"
      rel="stylesheet"
    />
    <style>
      :root {
        --bg: #f0f2f5;
        --card: #ffffff;
        --text: #1a1f2e;
        --muted: #57606a;
        --border: #d0d7de;
        --accent: #f97316;
      }

      * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
      }

      body {
        background: var(--bg);
        color: var(--text);
        font-family: "Outfit", sans-serif;
        padding: 28px 16px 48px;
      }

      .page {
        max-width: 980px;
        margin: 0 auto;
        background: var(--card);
        border: 1px solid var(--border);
        border-radius: 16px;
        overflow: hidden;
        box-shadow: 0 4px 24px rgba(0, 0, 0, 0.07);
      }

      .header {
        text-align: center;
        padding: 32px 20px 0;
      }

      .header h1 {
        margin: 0 0 8px;
        font-size: 28px;
        font-weight: 700;
      }

      .tagline {
        margin: 6px 0 18px;
        color: var(--accent);
        font-weight: 600;
        letter-spacing: 0.2px;
      }

      .button-row {
        display: flex;
        flex-wrap: wrap;
        gap: 8px;
        justify-content: center;
        margin-top: 28px;
      }

      .btn {
        padding: 8px 18px;
        border-radius: 8px;
        font-size: 12px;
        font-weight: 700;
        font-family: "Outfit", sans-serif;
        letter-spacing: 0.08em;
        text-transform: uppercase;
        text-decoration: none;
        color: #fff;
        transition: transform 0.15s, box-shadow 0.15s;
        display: inline-flex;
        align-items: center;
        gap: 6px;
      }

      .btn:hover {
        transform: translateY(-2px);
        box-shadow: 0 6px 18px rgba(0, 0, 0, 0.3);
      }

      .btn.blue {
        background: linear-gradient(135deg, #0969da, #1d4ed8);
      }

      .btn.orange {
        background: linear-gradient(135deg, #f97316, #ea580c);
      }

      .btn.red {
        background: linear-gradient(135deg, #cf222e, #b91c1c);
      }

      .btn.dark {
        background: linear-gradient(135deg, #24292f, #374151);
        border: 1px solid #555;
      }

      .body-content {
        padding: 32px 36px 44px;
      }

      .section {
        margin-top: 28px;
      }

      .section-title {
        font-size: 18px;
        font-weight: 700;
        display: flex;
        align-items: center;
        gap: 8px;
        margin-bottom: 14px;
        padding-bottom: 10px;
        border-bottom: 1px solid var(--border);
      }

      .muted {
        color: var(--muted);
        font-size: 14px;
        line-height: 1.7;
        margin-bottom: 10px;
      }

      .stack-grid {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 14px;
      }

      .stack-card {
        border: 1px solid var(--border);
        border-radius: 10px;
        padding: 16px;
        background: #fafbfc;
        transition: box-shadow 0.2s, border-color 0.2s;
      }

      .stack-card:hover {
        box-shadow: 0 4px 16px rgba(0, 0, 0, 0.08);
        border-color: #b0b8c2;
      }

      .stack-card h4 {
        font-size: 12px;
        font-weight: 700;
        text-transform: uppercase;
        letter-spacing: 0.08em;
        color: var(--muted);
        margin-bottom: 12px;
        font-family: "JetBrains Mono", monospace;
      }

      .body-badge-row {
        display: flex;
        flex-wrap: wrap;
        gap: 6px;
      }

      .bbadge {
        display: inline-flex;
        align-items: center;
        gap: 5px;
        padding: 4px 10px;
        border-radius: 5px;
        font-size: 12px;
        font-weight: 600;
        font-family: "JetBrains Mono", monospace;
        cursor: default;
        transition: transform 0.12s, opacity 0.12s;
      }

      .bbadge:hover {
        transform: scale(1.06);
      }

      .bbadge .dot {
        width: 7px;
        height: 7px;
        border-radius: 50%;
        flex-shrink: 0;
      }

      .bb-java {
        background: #fff3e0;
        color: #c2410c;
        border: 1px solid #fed7aa;
      }

      .bb-java .dot {
        background: #f89820;
      }

      .bb-jakarta {
        background: #fef2f2;
        color: #b91c1c;
        border: 1px solid #fecaca;
      }

      .bb-jakarta .dot {
        background: #dc2626;
      }

      .bb-spring {
        background: #f0fdf4;
        color: #15803d;
        border: 1px solid #bbf7d0;
      }

      .bb-spring .dot {
        background: #6db33f;
      }

      .bb-play {
        background: #f0fdf4;
        color: #166534;
        border: 1px solid #86efac;
      }

      .bb-play .dot {
        background: #16a34a;
      }

      .bb-unomi {
        background: #f5f3ff;
        color: #6d28d9;
        border: 1px solid #ddd6fe;
      }

      .bb-unomi .dot {
        background: #7c3aed;
      }

      .bb-python {
        background: #eff6ff;
        color: #1d4ed8;
        border: 1px solid #bfdbfe;
      }

      .bb-python .dot {
        background: #3b82f6;
      }

      .bb-react {
        background: #ecfeff;
        color: #0e7490;
        border: 1px solid #a5f3fc;
      }

      .bb-react .dot {
        background: #61dafb;
      }

      .bb-ts {
        background: #eff6ff;
        color: #1e40af;
        border: 1px solid #bfdbfe;
      }

      .bb-ts .dot {
        background: #3178c6;
      }

      .bb-js {
        background: #fefce8;
        color: #92400e;
        border: 1px solid #fef08a;
      }

      .bb-js .dot {
        background: #f7df1e;
      }

      .bb-html {
        background: #fff7ed;
        color: #c2410c;
        border: 1px solid #fed7aa;
      }

      .bb-html .dot {
        background: #e34c26;
      }

      .bb-css {
        background: #eff6ff;
        color: #1d4ed8;
        border: 1px solid #bfdbfe;
      }

      .bb-css .dot {
        background: #264de4;
      }

      .bb-mongo {
        background: #f0fdf4;
        color: #14532d;
        border: 1px solid #bbf7d0;
      }

      .bb-mongo .dot {
        background: #4db33d;
      }

      .bb-redis {
        background: #fef2f2;
        color: #b91c1c;
        border: 1px solid #fecaca;
      }

      .bb-redis .dot {
        background: #dc382d;
      }

      .bb-elastic {
        background: #fefce8;
        color: #854d0e;
        border: 1px solid #fef08a;
      }

      .bb-elastic .dot {
        background: #ffb703;
      }

      .bb-snowflake {
        background: #ecfeff;
        color: #155e75;
        border: 1px solid #a5f3fc;
      }

      .bb-snowflake .dot {
        background: #29b6f6;
      }

      .bb-s3 {
        background: #fff7ed;
        color: #9a3412;
        border: 1px solid #fdba74;
      }

      .bb-s3 .dot {
        background: #ff9900;
      }

      .bb-pg {
        background: #eff6ff;
        color: #1e40af;
        border: 1px solid #bfdbfe;
      }

      .bb-pg .dot {
        background: #336791;
      }

      .bb-mysql {
        background: #ecfeff;
        color: #164e63;
        border: 1px solid #a5f3fc;
      }

      .bb-mysql .dot {
        background: #00758f;
      }

      .bb-aws {
        background: #fff7ed;
        color: #9a3412;
        border: 1px solid #fdba74;
      }

      .bb-aws .dot {
        background: #ff9900;
      }

      .bb-docker {
        background: #eff6ff;
        color: #1d4ed8;
        border: 1px solid #bfdbfe;
      }

      .bb-docker .dot {
        background: #2496ed;
      }

      .bb-k8s {
        background: #eff6ff;
        color: #1e40af;
        border: 1px solid #bfdbfe;
      }

      .bb-k8s .dot {
        background: #326ce5;
      }

      .bb-jenkins {
        background: #fef2f2;
        color: #b91c1c;
        border: 1px solid #fecaca;
      }

      .bb-jenkins .dot {
        background: #d33726;
      }

      .bb-argo {
        background: #fdf4ff;
        color: #7e22ce;
        border: 1px solid #e9d5ff;
      }

      .bb-argo .dot {
        background: #ee82ee;
      }

      .bb-linux {
        background: #fefce8;
        color: #713f12;
        border: 1px solid #fef08a;
      }

      .bb-linux .dot {
        background: #f7c900;
      }

      .bb-kafka {
        background: #f8fafc;
        color: #374151;
        border: 1px solid #e2e8f0;
      }

      .bb-kafka .dot {
        background: #6b7280;
      }

      .bb-flink {
        background: #fef2f2;
        color: #b91c1c;
        border: 1px solid #fecaca;
      }

      .bb-flink .dot {
        background: #e23e57;
      }

      .bb-prom {
        background: #fff7ed;
        color: #c2410c;
        border: 1px solid #fed7aa;
      }

      .bb-prom .dot {
        background: #e6522c;
      }

      .bb-otel {
        background: #f8fafc;
        color: #475569;
        border: 1px solid #e2e8f0;
      }

      .bb-otel .dot {
        background: #94a3b8;
      }

      .bb-grafana {
        background: #fff7ed;
        color: #c2410c;
        border: 1px solid #fed7aa;
      }

      .bb-grafana .dot {
        background: #f46800;
      }

      .bb-shell {
        background: #f0fdf4;
        color: #14532d;
        border: 1px solid #bbf7d0;
      }

      .bb-shell .dot {
        background: #22c55e;
      }

      .bb-maven {
        background: #fef2f2;
        color: #b91c1c;
        border: 1px solid #fecaca;
      }

      .bb-maven .dot {
        background: #c71a36;
      }

      .list {
        margin: 0;
        padding-left: 0;
        list-style: none;
        color: var(--muted);
        font-size: 13.5px;
      }

      .list li {
        padding: 6px 0;
        border-bottom: 1px solid #f0f2f5;
        display: flex;
        align-items: flex-start;
        gap: 8px;
      }

      .list li:last-child {
        border-bottom: none;
      }

      .list li::before {
        content: "→";
        color: var(--accent);
        flex-shrink: 0;
        font-weight: 700;
      }

      .list a {
        color: inherit;
        text-decoration: none;
      }

      .list a:hover {
        text-decoration: underline;
      }

      .cta-section {
        margin-top: 32px;
        background: linear-gradient(135deg, #f9fafb, #f0f2f5);
        border: 1px solid var(--border);
        border-radius: 12px;
        padding: 24px;
        text-align: center;
      }

      .cta-section p {
        font-size: 14px;
        color: var(--muted);
        margin-bottom: 8px;
      }

      .cta-section p:last-child {
        margin-bottom: 0;
      }

      .cta-section strong {
        color: var(--text);
      }

      @media (max-width: 720px) {
        .stack-grid {
          grid-template-columns: 1fr 1fr;
        }

        .body-content {
          padding: 24px 20px 36px;
        }
      }

      @media (max-width: 480px) {
        .stack-grid {
          grid-template-columns: 1fr;
        }
      }
    </style>
  </head>
  <body>
    <main class="page">
      <section id="profile-header" class="header">
        <h1>👋 Hey there, I'm Shubham Gore !</h1>
        <div class="tagline">Software Developer | Java | Back-end</div>
        <div class="tagline">NoSQL | SQL | Spring | Kafka</div>
        <div class="tagline">
          Microservices | Distributed Systems | Open-Source Enthusiast
        </div>
        <div class="button-row" id="profile-links">
          <a class="btn blue" href="https://www.linkedin.com/in/shubham-gore-b02295230/"
            >LinkedIn</a
          >
          <a class="btn orange" href="https://hashnode.com/@shubhamagore">Blog</a>
          <a class="btn red" href="mailto:shubhamgore5454@gmail.com">Email</a>
          <a class="btn dark" href="https://github.com/shubhamagore">GitHub</a>
        </div>
      </section>

      <div class="body-content">
        <section id="about-me" class="section">
          <h2 class="section-title">🌟 About Me</h2>
          <p class="muted">
            Backend engineer with <strong>3+ years of experience</strong> building
            scalable Java microservices and distributed systems. I specialize in
            event-driven architectures, low-latency APIs, and cloud-native
            deployments with Docker, Kubernetes, and AWS.
          </p>
          <p class="muted">
            I focus on performance, reliability, and production ownership,
            working across Kafka-based systems, real-time pipelines, and data
            platforms backed by SQL and NoSQL stores.
          </p>
          <p class="muted">
            📧 Get in touch:
            <a href="mailto:shubhamgore5454@gmail.com">shubhamgore5454@gmail.com</a>
          </p>
        </section>

        <section id="blog-posts" class="section">
          <h2 class="section-title">📝 Latest Blog Posts</h2>
          <p class="muted" style="margin-bottom: 12px;">
            Writing about Java, cloud-native architectures, and open source
          </p>
          <ul class="list">
            <li>
              <a href="https://kafkaadvance.hashnode.dev/learning-kafka-advanced-journey-with-shubham-gore"
                >Learning Kafka: Advanced Journey With Shubham Gore</a
              >
            </li>
            <li>
              <a href="https://apachekafkain14days.hashnode.dev/learning-kafka-week-1-of-14-day-journey-with-shubham-gore"
                >Learning Kafka: Week 1 of 14-Day Journey</a
              >
            </li>
          </ul>
        </section>

        <section id="tech-stack" class="section">
          <h2 class="section-title">🛠️ Tech Stack</h2>
          <div class="stack-grid">
            <div class="stack-card">
              <h4>Backend &amp; Cloud Native</h4>
              <div class="body-badge-row">
                <span class="bbadge bb-java"><span class="dot"></span>Java</span>
                <span class="bbadge bb-jakarta"
                  ><span class="dot"></span>Jakarta EE</span
                >
                <span class="bbadge bb-play"><span class="dot"></span>Play</span>
                <span class="bbadge bb-spring"
                  ><span class="dot"></span>Spring Boot</span
                >
                <span class="bbadge bb-unomi"
                  ><span class="dot"></span>Apache Unomi</span
                >
                <span class="bbadge bb-python"
                  ><span class="dot"></span>Python</span
                >
              </div>
            </div>

            <div class="stack-card">
              <h4>Frontend</h4>
              <div class="body-badge-row">
                <span class="bbadge bb-react"
                  ><span class="dot"></span>React</span
                >
                <span class="bbadge bb-ts"
                  ><span class="dot"></span>TypeScript</span
                >
                <span class="bbadge bb-js"
                  ><span class="dot"></span>JavaScript</span
                >
                <span class="bbadge bb-html"
                  ><span class="dot"></span>HTML5</span
                >
                <span class="bbadge bb-css"
                  ><span class="dot"></span>CSS3</span
                >
              </div>
            </div>

            <div class="stack-card">
              <h4>Databases</h4>
              <div class="body-badge-row">
                <span class="bbadge bb-mongo"
                  ><span class="dot"></span>MongoDB</span
                >
                <span class="bbadge bb-redis"
                  ><span class="dot"></span>Redis</span
                >
                <span class="bbadge bb-elastic"
                  ><span class="dot"></span>Elasticsearch</span
                >
                <span class="bbadge bb-snowflake"
                  ><span class="dot"></span>Snowflake</span
                >
                <span class="bbadge bb-s3"
                  ><span class="dot"></span>Amazon S3</span
                >
                <span class="bbadge bb-pg"
                  ><span class="dot"></span>PostgreSQL</span
                >
                <span class="bbadge bb-mysql"
                  ><span class="dot"></span>MySQL</span
                >
              </div>
            </div>

            <div class="stack-card">
              <h4>Cloud &amp; DevOps</h4>
              <div class="body-badge-row">
                <span class="bbadge bb-aws"><span class="dot"></span>AWS</span>
                <span class="bbadge bb-docker"
                  ><span class="dot"></span>Docker</span
                >
                <span class="bbadge bb-k8s"
                  ><span class="dot"></span>Kubernetes</span
                >
                <span class="bbadge bb-jenkins"
                  ><span class="dot"></span>Jenkins</span
                >
                <span class="bbadge bb-argo"
                  ><span class="dot"></span>ArgoCD</span
                >
                <span class="bbadge bb-linux"
                  ><span class="dot"></span>Linux</span
                >
              </div>
            </div>

            <div class="stack-card">
              <h4>Messaging &amp; Data</h4>
              <div class="body-badge-row">
                <span class="bbadge bb-kafka"
                  ><span class="dot"></span>Apache Kafka</span
                >
                <span class="bbadge bb-flink"
                  ><span class="dot"></span>Apache Flink</span
                >
              </div>
            </div>

            <div class="stack-card">
              <h4>Tools &amp; Others</h4>
              <div class="body-badge-row">
                <span class="bbadge bb-prom"
                  ><span class="dot"></span>Prometheus</span
                >
                <span class="bbadge bb-otel"
                  ><span class="dot"></span>OpenTelemetry</span
                >
                <span class="bbadge bb-grafana"
                  ><span class="dot"></span>Grafana</span
                >
                <span class="bbadge bb-shell"
                  ><span class="dot"></span>Shell</span
                >
                <span class="bbadge bb-maven"
                  ><span class="dot"></span>Maven</span
                >
              </div>
            </div>
          </div>
        </section>

        <div class="cta-section">
          <p>💡 Open to collaboration and new challenges!</p>
          <p>⭐ <strong>Liked my work?</strong> Consider starring my repositories!</p>
          <p>🤝 <strong>Let's connect?</strong> Feel free to follow me or reach out!</p>
        </div>
      </div>
    </main>
  </body>
</html>
