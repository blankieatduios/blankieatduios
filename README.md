# Hi there! 👋 I'm blankieatduios

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&width=435&lines=Software+Developer;Problem+Solver;Open+Source+Enthusiast" alt="Typing SVG" />
</p>

## 🚀 About Me
A passionate developer dedicated to creating efficient and innovative solutions. I love exploring new technologies and contributing to the open-source community.

### 🛠️ Technologies & Tools
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=Python&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/-VS%20Code-007ACC?style=flat-square&logo=visual-studio-code&logoColor=white)
![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github)

### 📈 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=blankieatduios&show_icons=true&theme=dark" alt="GitHub Stats" />
</p>

### 🌱 Current Focus
- Expanding my knowledge in software development
- Contributing to open-source projects
- Building innovative solutions
- Collaborating with other developers

### 📫 How to Reach Me
- GitHub: [@blankieatduios](https://github.com/blankieatduios)
<!-- Add other social media links as needed -->

### ⚡ Fun Fact
When I'm not coding, you can find me exploring new technologies and learning about the latest tech trends!

---

name: Generate Snake Animation

on:
  schedule:
    - cron: "0 */12 * * *" # runs every 12 hours
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v3
      
      - uses: Platane/snk@v3
        id: snake-gif
        with:
          github_user_name: blankieatduios
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark
            dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9

      - name: Push to GitHub
        uses: EndBug/add-and-commit@v9
        with:
          branch: main
          message: 'Generate snake animation'
          add: 'dist'

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=blankieatduios&color=blue" alt="Profile views" />
</p>

> "Code is like humor. When you have to explain it, it's bad." – Cory House
