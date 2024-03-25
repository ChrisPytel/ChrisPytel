<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- Meta Information -->
    <title>Tweeter - Home Page</title>

    <!-- External CSS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css" type="text/css" />

    <!---External Fonts from Google -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Bungee&family=Source+Sans+3:ital,wght@0,200..900;1,200..900&display=swap" rel="stylesheet">

    <!-- External FontAwesome Assets -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />

    <!-- App CSS -->
    <link rel="stylesheet" href="/styles/layout.css" type="text/css" />
    <link rel="stylesheet" href="styles/nav.css" type="text/css" />
    <link rel="stylesheet" href="styles/header.css" type="text/css" />
    <link rel="stylesheet" href="styles/main.css" type="text/css" />
    <link rel="stylesheet" href="styles/new-tweet.css" type="text/css" />
    <link rel="stylesheet" href="styles/tweet.css" type="text/css" />

    <!-- External JS -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>

    <!-- App JS -->
    <script type="text/javascript" src="./scripts/client.js"></script>
    <script type="text/javascript" src="./scripts/composer-char-counter.js"></script>

  </head>
  <body>

    <nav>
      <div class="nav-container">
        <span class="nav-title">tweeter</span>
        <div class="nav-new-tweet">
          <span><b>Write</b> a new tweet</span>
          <i class="fa-solid fa-angles-down"></i>
        </div>
      </div>
    </nav>

    <header class ="orange-bg">
      <div>
          <img src="/images/profile-hex.png"> 
      </div>
      <div>
        <h2>Your Name</h2>
      </div>
    </header>  

  
    <main class="wrapper">

      <section class="new-tweet">
        <h2>Alright peeps listen up</h2>
        <form method="POST" action="/tweets"> 
          <textarea placeholder="I gotta tell ya something..." name="text" id="tweet-text"></textarea>
          <div class="divider"></div>
          <div class="below-line">
            <button class="tweet-button" type="submit">Tweet</button>
            <output class="counter" name="counter" for="tweet-text">140</output>
          </div>
        </form>
      </section>

      <section class="tweet-container wrapper">

        <article class="tweet">
          <header>
            <img src="/images/profile-hex.png">   
            <h3 class="person-title">Julius Ceasar</h3>
            <h3 class="handle">@Emperor4Life</h3>
          </header>
          <div>
            <p>Acta, non verba, Carthago delenda est. Veni, vidi, vici!</p>
          </div>
          <div class="divider">
          </div>
          <footer>
            <h6>X days ago</h6>
            <i class="fa-solid fa-flag"></i>
            <i class="fa-solid fa-retweet"></i>
            <i class="fa-solid fa-heart"></i>
          </footer> 
      </article>

      <article class="tweet">
        <header>
          <img src="/images/profile-hex.png">   
          <h3 class="person-title">Queen Victoria</h3>
          <h3 class="handle">@BritanniaRules</h3>
        </header>
        <div>
          <p>We are not interested in the possibilities of defeat. They do not exist.</p>
        </div>
        <div class="divider">
        </div>
        <footer>
          <h6>X days ago</h6>
          <i class="fa-solid fa-flag"></i>
          <i class="fa-solid fa-retweet"></i>
          <i class="fa-solid fa-heart"></i>
        </footer> 
    </article>
      
      </section>             
 
    </main>

  </body>
</html>
