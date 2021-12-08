## Olá, Bem-Vindo(a), é um prazer te ter aqui! 😁

- 🎂 18 Anos
- 💼 Aberto para novas oportunidades.
- ❤️ Gosto de Front-end e Back-end.
- 📖 Atualmente cursando Análise e Desenvolvimento de Sistemas

<div>

##

#### 🤖 Minha atividade no GitHub
  
<div style="display: inline_block;">
  <a href="https://github.com/BrunoCason">
  <img height="140em" src="https://github-readme-stats.vercel.app/api?username=BrunoCason&show_icons=true&theme=gotham&include_all_commits=true&count_private=true"/>
  <img height="140em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=BrunoCason&layout=compact&langs_count=7&theme=gotham"/>
</div>
  
<div style="display: inline_block"><br>
  <img align="center" alt="Andre-HTML" height="30" width="30" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="Andre-CSS" height="30" width="30" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img align="center" alt="Andre-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="right" alt="Andre-pic" height="145" style="border-radius:80px," src="https://github.com/AndreWar10/AndreWar10/blob/main/dormrm.gif">

  ##
 
<div> 
  <a href="https://instagram.com/andre.guerra02" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a> 
  <a href="https://api.whatsapp.com/send/?phone=5516992062879&text&app_absent=0" target="_blank"><img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" target="_blank"></a> 
  <a href = "mailto:andreguerra.2002@hotmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/andr%C3%A9-guerra-santos-b54b281b6/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
 
  ![Snake animation](https://github.com/rafaballerini/rafaballerini/blob/output/github-contribution-grid-snake.svg)
 
</div>

.....................................................................

......................................................................

cobrinha
name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
