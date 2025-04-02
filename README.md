# Aidan Corcoran - Personal Portfolio Website

[![CI/CD Status](https://github.com/aidancorcoran/portfolio/actions/workflows/deploy.yml/badge.svg)](https://github.com/aidancorcoran/portfolio/actions/workflows/deploy.yml)
This repository contains the source code for my personal portfolio website, showcasing my skills, professional experience, and projects as a Software Engineer based in Toronto, Canada.

🌐 **Live Demo:** [https://aidancorcoran.dev](https://aidancorcoran.dev)

## ✨ Features

* **Responsive Design:** Adapts to various screen sizes using Tailwind CSS.
* **Single Page Application:** Smooth scrolling navigation between sections.
* **Dynamic Content:** JavaScript for mobile menu toggle and dynamic footer year.
* **Key Sections:**
    * Home: Introduction and call to action.
    * About Me: Background, education, and current roles.
    * Skills: Detailed list of programming languages and technologies.
    * Experience: Professional work history.
    * Projects: Showcase of personal and professional projects (FrameMax, GDrive CLI).
    * Contact: Links to social profiles (GitHub, LinkedIn), email, and a functional contact form via Formspree.

## 🛠️ Technologies Used

* **Frontend:**
    * HTML5
    * [Tailwind CSS](https://tailwindcss.com/) (via CDN)
    * Vanilla JavaScript (for UI interactions)
    * [Inter Font](https://rsms.me/inter/)
* **Icons:**
    * [Lucide Icons](https://lucide.dev/) (via CDN font)
    * [Simple Icons](https://simpleicons.org/) (via CDN SVG links)
* **Contact Form Backend:**
    * [Formspree](https://formspree.io/)

## 🚀 Deployment

This website is automatically deployed using a CI/CD pipeline configured with GitHub Actions:

1.  **Trigger:** Pushes to the `main` branch initiate the deployment workflow defined in `.github/workflows/deploy.yml`.
2.  **Build/Sync:** The workflow checks out the repository code.
3.  **AWS Sync:** It uses `aws s3 sync` to upload the website files (excluding `.git/` and `.github/` directories) to an AWS S3 bucket configured for static website hosting. The `--delete` flag ensures the bucket mirrors the repository content.
4.  **Serving:** [Cloudflare](https://www.cloudflare.com/) sits in front of the S3 bucket, providing:
    * DNS resolution for `aidancorcoran.dev`.
    * CDN caching for improved performance.
    * Free SSL/TLS encryption (HTTPS).

## 🔧 Local Development

No complex build process is required for local viewing:

1.  Clone the repository:
    ```bash
    git clone [https://github.com/aidancorcoran/aidancorcoran.github.io.git](https://www.google.com/search?q=https://github.com/aidancorcoran/aidancorcoran.github.io.git)
    # TODO: Replace with your actual repo URL
    cd aidancorcoran.github.io
    ```
2.  Open the `index.html` file directly in your web browser.

## 📫 Contact

* **Website:** [aidancorcoran.dev](https://aidancorcoran.dev)
* **GitHub:** [@aidancorcoran](https://github.com/aidancorcoran)
* **LinkedIn:** [Aidan Corcoran](https://www.linkedin.com/in/aidan-corcoran-99b691203/)
* **Email:** aidancorcoran.dev@gmail.com

---

&copy; 2025 Aidan Corcoran. All Rights Reserved.