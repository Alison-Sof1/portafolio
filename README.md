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
            <a class="list-item__link" href="#home">INICIO</a>
          </li>
          <li class="main-list__item list-item">
            <a class="list-item__link" href="#about">ACERCA DE</a>
          </li>
          <li class="main-list__item list-item">
            <a class="list-item__link" href="#skills">HABILIDADES</a>
          </li>
        </ul>
      </nav>
    </header>
    <main class="main">
      <!-- Vista previa -->
      <section class="main__home home" id="home">
        <h1 class="home__title">ALISON PEÑUELA</h1>
        <p class="home__subtitle">DESARROLLADOR WEB, PROGRAMADOR PYTHON</p>
      </section>
      <!-- Acerca de mí -->
      <section class="main__about about" id="about">
        <h2 class="about__title">SOBRE MI!</h2>
        <div class="about__info info-block">
          <p class="info-block__text">
            Soy Ali mas apodada como Sof1(virtualmente), tengo 12 años, Naci en Colombia-Tolima. Me uni a programacion por que me gusta crear juegos, como crear modelos u aportar ideas.
            En Python Basico hice un juego parecido como el Dinosaur Game,actualmente soy programadora de Py-pro. Me gusta mucho: dibujar,me gusta el idioma ingles,tambien amo las matematicas
            entreno basquetbol,soy amistosx,me gusta escuchar musica(como la de ingles,electronica y clasica),me gusta el piano, en algun tiempo estuve en clases de piano en cual quiero retomar
            nuevamente y soy youtuber y tiktoker, solo eso, grax :3 
          </p>
          <img
            class="info-block__img"
            src="../static/img/profile.png"
            alt="me"
            width="250"
            height="250"
          />
        </div>
      </section>
      <!-- Sección de competencias -->
      <section class="main__skills skills" id="skills">
        <h2 class="skills__title">MIS HABILIDADES</h2>
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
              <span class="skill__info">python</span>
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
              <span class="skill__info">Discord</span>
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
              <span class="skill__info">HTML</span>
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
              <span class="skill__info">Base de datos</span>
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
            <input type="email" class="form__input" name="email" id="email" placeholder="Ingrese su E-mail" required>
          </label>
          <label for="text">
            <textarea name="text" class="form__input" id="text" cols="70" rows="10" required placeholder="Comentario..."></textarea>
          </label>
          <button class="form__button" type="submit">ENVIAR</button>
        </form>
      </section>
    </main>
    <!-- Pie de página con enlaces a redes sociales -->
    <footer>

    </footer>
  </body>
</html>
