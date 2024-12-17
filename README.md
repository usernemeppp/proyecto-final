<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta
      name="viewport"
      content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0"
    />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="../static/css/style.css" />
    <title>Portafolio</title>
  </head>
  <body>
     <header class="header">
      <nav class="header__nav main-nav">
        <ul class="main-nav__list main-list">
          <li class="main-list__item list-item">
            <a class="list-item__link" href="#home">HOME</a>
          </li>
          <li class="main-list__item list-item">
            <a class="list-item__link" href="causes">CAUSES</a>
          </li>
          <li class="main-list__item list-item">
           <a class="list-item__link" href="#skills">MY SKILLS</a>
          </li>
        </li>
      </nav>
    </header>
    <main class="main">
      <!-- Vista previa -->
      <section class="main__home home" id="home">
        <h1 class="home__title"> Climate Change        
        </h1>
        <p class="home__subtitle">Climate change refers to long-term changes in temperatures and weather patterns. These changes can be natural, due to variations in solar activity or large volcanic eruptions. But since the 19th century, human activities have been the main driver of climate change, mainly due to the burning of fossil fuels such as coal, oil and gas.
          The burning of fossil fuels generates greenhouse gas emissions that act like a blanket that envelops the Earth, trapping the sun's heat and raising temperatures.
          </p>
        </section>
        <h1 class="causes__title">causes</h1>
      </section>
      <!-- Sección de competencias -->
      <section class="main__skills skills" id="skills">
        <h2 class="skills__title">MY SKILLS</h2>
        <form action="/" method="POST">
          <ul class="skills__list skills-list">
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/python.png"
                alt="python"
                width="150"
                height="150"
              />
              <span class="skill__info">Skill info</span>
              <input class="skill__button" type="submit" name="button_python" value="SHOW PROJECT">
            </li>
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/discord.png"
                alt="discord"
                width="150"
                height="150"
              />
              <span class="skill__info">Skill info</span>
              <input class="skill__button" type="submit" name="button_discord" value="SHOW PROJECT">
            </li>
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/html.png"
                alt="html"
                width="150"
                height="150"
              />
              <span class="skill__info">Skill info</span>
              <input class="skill__button" type="submit" name="button_html" value="SHOW PROJECT">
            </li>
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/db.webp"
                alt="SQL"
                width="150"
                height="150"
              />
              <span class="skill__info">Skill info</span>
              <input class="skill__button" type="submit" name="button_db" value="SHOW PROJECT">
            </li>
          </ul>
        </form>
        {% if button_python%}
          <div class="skills__project project" id="project">
              <img class="project__img" src="../static/img/python-project.png" alt="project" width="500">
              <a class="project__link" href="">Abierto en GitHub</a>
          </div>
        {% endif %}
      </section>
      <!-- Formulario de contacto -->
      <section class="main__feedback feedback" id="feedback">
        <h2 class="feedback__title">FEEDBACK</h2>
        <form action="" method="POST" class="feedback__form form">
          <label for="email">
            <input type="email" class="form__input" name="email" id="email" placeholder=" E-mail" required>
          </label>
          <label for="text">
            <textarea name="text" class="form__input" id="text" cols="70" rows="10" required placeholder="Comment"></textarea>
          </label>
          <button class="form__button" type="submit">SEND</button>
        </form>
      </section>
    </main>
    <!-- Pie de página con enlaces a redes sociales -->
    <footer>

    </footer>
  </body>
</html>

