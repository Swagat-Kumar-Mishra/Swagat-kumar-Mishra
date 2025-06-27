<!-- ELEGANT MINIMALIST THEME - BY AI -->

<div style="font-family: 'Inter', 'Segoe UI', 'Helvetica Neue', 'Arial', sans-serif; width: 100%; padding: 10px;">

<!-- Header: Name & Title -->
<div style="text-align: left; margin-bottom: 50px;">
  <h1 style="font-weight: 800; font-size: 4em; margin-bottom: 0px;">
    <span style="background: -webkit-linear-gradient(45deg, #BE58CB, #F27979); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
      Swagat Mishra.
    </span>
  </h1>
  <p style="font-size: 1.5em; font-weight: 300; color: #E0D2E4; margin-top: 5px;">
    Full-Stack Developer & Cloud Architect
  </p>
</div>

<!-- Section: About & Stats -->
<table width="100%" style="border: none;">
  <tr>
    <!-- Left Column: About Me -->
    <td width="60%" valign="top" style="padding-right: 20px;">
      <h2 style="font-weight: 600; color: #BE58CB; border-bottom: 1px solid #444; padding-bottom: 10px;">// ABOUT</h2>
      <p style="color: #E0D2E4; font-size: 1.1em; line-height: 1.6;">
        I'm a software engineer who builds robust, scalable, and elegant digital experiences. My passion lies in solving complex problems with clean code and architecting systems that stand the test of time.
        <br><br>
        Currently focused on distributed systems, cloud-native technologies, and refining my craft through continuous learning.
      </p>
    </td>
    
    <!-- Right Column: Stats -->
    <td width="40%" valign="top" style="padding-left: 20px;">
        <img src="https://github-readme-stats.vercel.app/api?username=Swagat-Kumar-Mishra&show_icons=true&theme=transparent&bg_color=00000000&title_color=BE58CB&text_color=E0D2E4&icon_color=F27979&border_color=444" alt="Swagat's GitHub Stats"/>
        <img src="https://github-readme-streak-stats.herokuapp.com?user=Swagat-Kumar-Mishra&theme=transparent&background=00000000&border=444&stroke=BE58CB&ring=F27979&fire=F27979&currStreakNum=E0D2E4&sideNums=E0D2E4&currStreakLabel=E0D2E4&sideLabels=E0D2E4&dates=E0D2E4" alt="Swagat's GitHub Streak"/>
    </td>
  </tr>
</table>

<hr style="border-color: #444; margin: 50px 0;">

<!-- Section: Toolkit -->
<div>
  <h2 style="font-weight: 600; color: #BE58CB; border-bottom: 1px solid #444; padding-bottom: 10px;">// TOOLKIT</h2>
  <p align="center" style="margin-top: 30px;">
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5"/>
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3"/>
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
    <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin"/>
    <img src="https://img.shields.io/badge/Swift-FA7343?style=for-the-badge&logo=swift&logoColor=white" alt="Swift"/>
  </p>
</div>

<hr style="border-color: #444; margin: 50px 0;">

<!-- Section: Activity -->
<div align="center">
  <h2 style="font-weight: 600; color: #BE58CB;">// ACTIVITY</h2>
  <!-- Contribution Snake -->
  <img src="https://github.com/Swagat-Kumar-Mishra/Swagat-Kumar-Mishra/blob/output/github-contribution-grid-snake.svg" alt="Contribution Snake" style="margin-top: 20px;">
</div>

</div>

---

### ⚠️ Setup Required: Contribution Snake Animation

The contribution snake animation (`github-contribution-grid-snake.svg`) **will not show up automatically**. You need to set up a simple GitHub Action to generate it. If you have already done this, you can ignore this step.

**How to set it up:**

1.  **Create a folder path:** In your profile repository (`Swagat-Kumar-Mishra/Swagat-Kumar-Mishra`), create a new folder named `.github`. Inside that, create another folder named `workflows`.
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
4.  **Commit the changes:** Save and commit the new file. The action will run automatically. Once it runs, the animation will appear on your profile.
