# 🌐 MitchFlix — Personal Website & Portfolio

**Live site:** [https://mitchflix.co.uk](https://mitchflix.co.uk)

This repository hosts the source code and configuration for my personal website **MitchFlix**, built as a central hub for my projects, homelab documentation, and space-tech learning journey.  

It’s deployed using **GitHub Pages** and secured with **Cloudflare**, with a custom domain and HTTPS enabled.

This run book show's you how I made it **for free** (other than buying the domain via GoDaddy)

---

## 🧩 Overview

**Goal:**  
To create a simple, reliable, and low-cost personal website to showcase my:
- 💻 Homelab builds and observability stack  
- 🚀 Space systems & comms experiments  
- 📊 Monitoring and automation projects  
- 🧠 Blog posts and technical writeups  
- 🔗 Links to GitHub, LinkedIn, Plex, and Discord

---

## ⚙️ Deployment Setup

### 1. Create the Repository
1. Created a new GitHub repo named `mitchflix`.
2. Added a simple `index.html` file to test deployment.
3. Enabled **GitHub Pages** in the repo settings:
   - Branch: `main`  
   - Folder: `/ (root)`  
   - GitHub automatically deployed the site to  
     `https://<username>.github.io/mitchflix/`.

---

### 2. Configure the Custom Domain
1. Purchased the domain **mitchflix.co.uk**.
2. Added it in the repo under **Settings → Pages → Custom domain**.
3. GitHub generated a `CNAME` file automatically.

---

### 3. Set Up Cloudflare
1. Created a **Cloudflare account** and added the domain.  
2. Updated my domain registrar to use **Cloudflare’s nameservers**.
3. Added two DNS records in Cloudflare:  
    - Type: A Name: @ Value: 185.199.108.153 (GitHub Pages IP)
     -Type: CNAME Name: www Value: <username>.github.io

4. Enabled:
- **Always Use HTTPS**
- **Automatic HTTPS Rewrites**
- **SSL/TLS → Full (Strict)**
- **Caching → Standard**

---

### 4. Verify HTTPS & Test
- Waited for DNS propagation (~10–15 mins).  
- Verified that `https://mitchflix.co.uk` resolves to GitHub Pages with a padlock.  
- Updated links and metadata in the HTML files.

---

## 🛠️ Stack

| Component        | Purpose                         |
|------------------|----------------------------------|
| **GitHub Pages** | Hosting static site              |
| **Cloudflare**   | DNS + HTTPS + CDN caching        |
| **Custom domain**| Professional branding & SEO      |
| **HTML/CSS**     | Simple, fast static layout       |

---

## 🧠 Lessons Learned

- GitHub Pages + Cloudflare = a **free and secure hosting stack**.  
- Custom domains need **DNS propagation time** — be patient!  
- Cloudflare’s **proxy + SSL** makes HTTPS setup almost effortless.  
- It’s worth documenting each step for future site updates or rebuilds.

---

## 🚀 Future Plans

- Add a **blog section** (Markdown to HTML auto-build).
- Integrate **GitHub Actions** for auto-deployment.
- Host API endpoints or monitoring dashboards later.
- Add a **space-tech projects** gallery page.

---

## 📬 Contact

- GitHub: [github.com/MitchMcLellan](https://github.com/MitchMcLellan)  
- LinkedIn: *coming soon*  
- Discord: *available on request*  
- Website: [https://mitchflix.co.uk](https://mitchflix.co.uk)

---

### 🛰️ “Built from the homelab, powered by curiosity.”

