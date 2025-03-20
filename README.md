# <p align="center">Hello there 👋, I am Rishab Kumar Pattnaik</p>
### <p align="center">Pre-Final Year Student at BITS Pilani Hyderabad Campus</p>

<table>
  <tr>
    <td width="60%">
      
## 🖥️ I work on Deep Learning, Computer Vision, Representation Learning, Generative AI. 🖥️ 

---

🔭 **Currently Working On**  
- Deep Learning research projects
- Computer Vision applications
- Open-source contributions
- AI/ML/Gen AI Applications

🌱 **Currently Learning**  
- Advanced Neural Networks
- Generative AI models
- Optimized model deployment
- MLOps
- Agentic AI
- Reinforcement Learning
    </td>
    <td width="40%">
      <img src="https://media.tenor.com/Lbfyti3y8UkAAAAM/machine-learning-artificial-intelligence.gif" width="100%" alt="Machine Learning GIF"/>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td width="60%">
      
💻 **Tech Stack & Tools**

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white)
![MLOps](https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![AutoML](https://img.shields.io/badge/AutoKeras-FF6F00?style=for-the-badge&logo=keras&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-65BBA9?style=for-the-badge&logo=ollama&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)

</div>
    </td>
    <td width="40%">
      <img src="https://media1.tenor.com/m/2uyENRmiUt0AAAAd/coding.gif" width="100%" alt="Coding GIF"/>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td width="60%">
      
📫 **Reach Me At**  
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rishabpattnaik9@gmail.com)
[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rishab-kumar-pattnaik-6a9939249/)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF7139?style=for-the-badge&logo=firefox-browser&logoColor=white)](https://riiishaab.github.io/)
    </td>
    <td width="40%">
      <img src="https://media.tenor.com/n53f5g-plM0AAAAj/emo.gif" width="100%" alt="Emo GIF"/>
    </td>
  </tr>
</table>

name: Generate Snake Animation

on:
  schedule:
    - cron: "0 */12 * * *" # Runs every 12 hours
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: Riiishaab
          svg_out_path: dist/github-contribution-grid-snake.svg
          svg_out_path_dark: dist/github-contribution-grid-snake-dark.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}



