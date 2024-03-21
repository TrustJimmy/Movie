<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Сайт кинотеатра</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@8/swiper-bundle.min.css">
  <script src="https://cdnjs.cloudflare.com/ajax/libs/Swiper/8.4.5/swiper-bundle.min.js"></script>
  <link rel="stylesheet" href="../src/lib/style.css">
</head>
<body>
  <section>
    <div class="swiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide swiper-slide--one">
          <span>Жанр: военный</span>
          <div>
            <h2>Воздух</h2>
            {#each film1 as link}
              <a href={link.href} class="link">{link.title}</a>  
            {/each}
          </div>
        </div>
        <div class="swiper-slide swiper-slide--two">
          <span>Жанр: драма</span>
          <div>
            <h2>Вызов</h2>
            {#each film2 as link}
              <a href={link.href} class="link">{link.title}</a>  
            {/each}
          </div>
        </div>
  
        <div class="swiper-slide swiper-slide--three">
          <span>Жанр: мелодрама</span>
          <div>
            <h2>Лёд 3</h2>
            {#each film3 as link}
              <a href={link.href} class="link">{link.title}</a>  
            {/each}
          </div>
        </div>
  
        <div class="swiper-slide swiper-slide--four">
          <span>Жанр: фэнтези</span>
          <div>
            <h2>Мастер и Маргарита</h2>
            {#each film4 as link}
              <a href={link.href} class="link">{link.title}</a>  
            {/each}
          </div>
        </div>
  
        <div class="swiper-slide swiper-slide--five">
          <span>Жанр: мелодрама</span>
          <div>
            <h2>Онегин</h2>
            {#each film5 as link}
              <a href={link.href} class="link">{link.title}</a>  
            {/each}
          </div>
        </div>
      </div>
      <div class="swiper-pagination"></div>
    </div>
  </section>

  <script src="../src/lib/index.js"></script>
</body>
</html>

<script>
    const film1 = [
        {
            title: 'Читать описание',
            href: '/vozduh',
        },
    ];
    const film2 = [
        {
            title: 'Читать описание',
            href: '/vizov',
        },
    ];
    const film3 = [
        {
            title: 'Читать описание',
            href: '/led',
        },
    ];
    const film4 = [
        {
            title: 'Читать описание',
            href: '/M&M',
        },
    ];
    const film5 = [
        {
            title: 'Читать описание',
            href: '/onegin',
        },
    ];
</script>