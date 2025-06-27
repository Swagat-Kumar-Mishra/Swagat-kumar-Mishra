<!-- NEON NOIR TERMINAL THEME - BY AI -->

<!-- Main container to create a layered effect -->
<div style="position: relative; width: 100%; height: 100%;">

<!-- 1. Animated Background Layer -->
<img src="https://media.giphy.com/media/g04h9gUj7P2uY/giphy.gif" alt="Rainy Neon City" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; object-fit: cover; opacity: 0.7;" />

<!-- 2. Content Layer -->
<div style="position: relative; z-index: 1; padding: 20px; background: rgba(0,0,0,0.5); backdrop-filter: blur(2px);">

<!-- Header Section: Glitch-on-Hover Profile -->
<div align="center" style="margin-bottom: 30px;">
  
  <!-- Glitch Container -->
  <div class="glitch-container" style="position: relative; display: inline-block; border-radius: 50%; padding: 5px; background: linear-gradient(45deg, #BE58CB, #F27979); animation: spin 4s linear infinite;">
    <a href="https://github.com/Swagat-Kumar-Mishra">
      <img src="https://github.com/Swagat-Kumar-Mishra.png" alt="Swagat Kumar Mishra" style="border-radius: 50%; width: 180px; height: 180px; border: 5px solid #101010;">
    </a>
    <!-- Glitch Overlay Layers -->
    <div class="glitch-overlay" style="--char-1: '█'; --char-2: '░'; --char-3: '▓';"></div>
  </div>

  <!-- CSS for Glitch Effect and Spinning Gradient Border -->
  <style>
    .glitch-container { transition: all 0.3s ease-in-out; }
    .glitch-overlay { position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 50%; pointer-events: none; opacity: 0; transition: opacity 0.3s; }
    .glitch-container:hover .glitch-overlay { opacity: 1; }
    .glitch-container:hover .glitch-overlay::before,
    .glitch-container:hover .glitch-overlay::after { content: var(--char-1) var(--char-2) var(--char-3); position: absolute; top: 0; left: 0; width: 100%; height: 100%; color: cyan; font-size: 3em; text-align: center; line-height: 180px; animation: glitch-anim 0.3s infinite; }
    .glitch-container:hover .glitch-overlay::after { color: magenta; animation-delay: 0.05s; }
    @keyframes glitch-anim { 0% { clip: rect(25px, 9999px, 92px, 0); } 20% { clip: rect(80px, 9999px, 150px, 0); } 40% { clip: rect(50px, 9999px, 100px, 0); } 60% { clip: rect(120px, 9999px, 80px, 0); } 80% { clip: rect(30px, 9999px, 130px, 0); } 100% { clip: rect(70px, 9999px, 90px, 0); } }
    @keyframes spin { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }
  </style>
  
  <br><br>
  <!-- Name and Typing Animation -->
  <h1 style="font-family: 'Courier New', Courier, monospace; font-weight: bold; font-size: 2.5em; color: #E0D2E4;">
    > Swagat Kumar Mishra
  </h1>
  <img src="https://readme-typing-svg.herokuapp.com?font=Courier+New&weight=700&size=24&color=00FF00¢er=true&vCenter=true&width=600&lines=Initializing+connection...;Accessing+main-frame...;Full-Stack+Developer+%7C%7C+Cloud+Architect" alt="Typing Animation">
</div>

<!-- Main Dashboard: Two-Column Layout -->
<table width="100%" style="border: none;">
  <tr>
    <!-- Left Column: System Core & Mission -->
    <td width="50%" valign="top" style="padding-right: 15px;">
      <h2 style="font-family: 'Courier New', Courier, monospace; color: #BE58CB;">//:ROOT> whoami</h2>
      <p style="font-family: 'Segoe UI', sans-serif; color: #E0D2E4; font-size: 1.1em;">
        A digital architect and problem-solver navigating the complexities of the web. I build high-performance, scalable systems and thrive on turning abstract ideas into tangible technology. My terminal is always open to new challenges.
      </p>
      <br>
      <h2 style="font-family: 'Courier New', Courier, monospace; color: #BE58CB;">//:SYSTEM_CORE</h2>
      <p align="left">
        <img src="https://img.shields.io/badge/HTML5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5"/>
        <img src="https://img.shields.io/badge/CSS3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3"/>
        <img src="https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
        <br><br>
        <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
        <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin"/>
        <img src="https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white" alt="Swift"/>
      </p>
    </td>
    
    <!-- Right Column: Data Streams -->
    <td width="50%" valign="top" style="padding-left: 15px;">
      <h2 style="font-family: 'Courier New', Courier, monospace; color: #BE58CB;" align="right">//:DATA_STREAMS</h2>
      <p align="center">
        <!-- Stats Card with Transparent BG -->
        <img src="https://github-readme-stats.vercel.app/api?username=Swagat-Kumar-Mishra&show_icons=true&include_all_commits=true&count_private=true&theme=tokyonight&bg_color=00000000&title_color=BE58CB&text_color=E0D2E4&icon_color=F27979&border_color=BE58CB&hide_border=false" alt="Swagat's GitHub Stats"/>
        <br>
        <!-- Streak Card with Transparent BG -->
        <img src="https://github-readme-streak-stats.herokuapp.com?user=Swagat-Kumar-Mishra&theme=tokyonight&background=00000000&border=BE58CB&stroke=BE58CB&ring=F27979&fire=F27979&currStreakNum=E0D2E4&sideNums=E0D2E4&currStreakLabel=E0D2E4&sideLabels=E0D2E4&dates=E0D2E4" alt="Swagat's GitHub Streak"/>
      </p>
    </td>
  </tr>
</table>

<!-- Footer: Activity Log -->
<div align="center" style="margin-top: 30px;">
  <!-- Neon Glitch Divider -->
  <img src="https://media.giphy.com/media/iIq2sY1YfV27T4sT1i/giphy.gif" width="100%">
  
  <h2 style="font-family: 'Courier New', Courier, monospace; color: #BE58CB;">//:ACTIVITY_LOG</h2>
  
  <!-- Contribution Snake -->
  <img src="https://github.com/Swagat-Kumar-Mishra/Swagat-Kumar-Mishra/blob/output/github-contribution-grid-snake-dark.svg" alt="Contribution Snake">
  
  <h3 style="font-family: 'Courier New', Courier, monospace; font-weight: 500; color: #00FF00; margin-top: 20px;">
    > Session terminated.
  </h3>
</div>

</div>
</div>

---

### ⚠️ Setup Required: Contribution Snake Animation

The contribution snake animation (`github-contribution-grid-snake-dark.svg`) **will not show up automatically**. You need to set up a simple GitHub Action to generate it for you.

**How to set it up (takes 2 minutes):**

1.  **Create a new repository folder:** In your profile repository (`Swagat-Kumar-Mishra/Swagat-Kumar-Mishra`), create a new folder named `.github`. Inside that folder, create another folder named `workflows`.
2.  **Create the action file:** Inside the `.github/workflows` folder, create a new file named `main.yml`.
3.  **Copy and paste the code:** Paste the following code into the `main.yml` file:
    ```yml
    name: Generate Snake Animation

    on:
      schedule:
        - cron: "0 */12 * * *" # Runs every 12 hours
      workflow_dispatch:

    jobs:
      generate:
        runs-on: ubuntu-latest
        steps:
          - name: Generate snake animation
            uses: Platane/snk/svg-only@v3
            with:
              github_user_name: ${{ github.repository_owner }}
              outputs: |
                dist/github-contribution-grid-snake.svg
                dist/github-contribution-grid-snake-dark.svg?palette=github-dark
            env:
              GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
    ```
4.  **Commit the changes:** Save and commit the new file. The action will run automatically every 12 hours (and you can also run it manually from the "Actions" tab of your repository).

Once the action has run for the first time, the snake animation will appear on your profile!
