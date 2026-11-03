## Hi there 👋

<!--
**l0r3ns/l0r3ns** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<div align="center">
  <!-- Contador de visitas -->
  <p>Visitor count</p>
  <img src="https://profile-counter.glitch.me/TU_USUARIO/count.svg" alt="Visitor's Count" />
</div>

<p align="center">
  <img src="https://github.com/TU_USUARIO/TU_USUARIO/blob/main/tu-banner.png" alt="Banner" width="100%">
</p>

<h1 align="center">
  <img src="https://readme-typing-svg.herokuapp.com/?font=Inter&size=36&center=true&vCenter=true&width=500&height=70&color=4493F8&duration=4000&lines=¡Hola,+Mundo!+👋;+Soy+Tu+Nombre;+Desarrollador+Full-Stack;" />
</h1>

## 🛠️ Tecnologías y Herramientas

<p align="center">
  <img src="https://skillicons.dev/icons?i=js,ts,react,nextjs,nodejs,python,docker,git,vscode" alt="Skills" />
</p>

<div align="center">
  <img width="390" src="https://github-readme-stats.vercel.app/api?username=TU_USUARIO&theme=transparent&show_icons=true&count_private=true" alt="Stats" />
  <img width="390" src="https://github-readme-streak-stats.herokuapp.com/?user=TU_USUARIO&theme=transparent" alt="Streak" />
</div>

name: Generate Snake
on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: Platane/snk@v3
        id: snake-gif
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

          <div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/TU_USUARIO/TU_USUARIO/output/github-contribution-grid-snake-dark.svg" />
    <img alt="github-snake" src="https://raw.githubusercontent.com/TU_USUARIO/TU_USUARIO/output/github-contribution-grid-snake.svg" />
  </picture>
</div>
