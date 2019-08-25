<template>
  <div>
    <header class="hero">
      <img
        class="hero__logo"
        src="~assets/images/portland_logo_coloured.svg"
        alt="Portland Brothers"
      />
      <!-- <h1 class="hero__heading">Portland Brothers</h1> -->
    </header>
    <main class="main">
      <div class="main__media">
        <article class="media">
          <header class="media__header">
            <h4 class="media__heading">Shake Off The Dust video</h4>
            <p>Hand stiched by Steve</p>
          </header>
          <div class="media__video">
            <iframe
              title="youtube player"
              width="560"
              height="315"
              src="https://www.youtube.com/embed/BXl7g7nqztU"
              frameborder="0"
              allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen
            ></iframe>
          </div>
        </article>
      </div>
      <div class="main__media">
        <article class="media">
          <header class="media__header">
            <h4 class="media__heading">First EP</h4>
            <p>Now on Spotify</p>
          </header>
          <div class="media__spotify">
            <iframe
              title="Spotify player"
              src="https://open.spotify.com/embed/album/0JSpmsF8C2xMPe8wmsSSJH"
              width="300"
              height="210"
              frameborder="0"
              allowtransparency="true"
              allow="encrypted-media"
            ></iframe>
          </div>
        </article>
      </div>
      <header class="main__header">
        <h1 class="main__heading">Portland Brothers</h1>
        <p>We are Steven Adams and Timothy Victor and we do songs.</p>
      </header>
      <p class="main__paragraph">
        Adams was in The Broken Family Band. TV produced their first two records
        and played with the band. A lot.
      </p>
      <p class="main__paragraph">
        We played together in The Singing Adams and made a record together
        called 'Problems'. TV also plays with his band The Folk Orchestra. Adams
        plays solo and with his band The French Drops.
      </p>
      <p class="main__paragraph">
        We first met in a pub called The Portland Arms.
      </p>
      <p class="main__paragraph">
        We like folk and pop and country and all the other types of music. Get
        in touch.
      </p>
      <ul class="link-list">
        <li class="link-list__item">
          <a class="link-list__link" href="mailto:singingadams@gmail.com"
            >Email</a
          >
        </li>
        <li class="link-list__item">
          <a class="link-list__link" href="https://twitter.com/portbros"
            >Twitter</a
          >
        </li>
        <!-- <li class="link-list__item">
          <a class="link-list__link" href="#">Discounted sex toys</a>
        </li>-->
      </ul>
    </main>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'The Portland Brothers',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'description',
          name: 'description',
          content:
            'Steven Adams (The French Drops, The Singing Adams and The Broken Family Band) and Timothy Victor (the Folk Orchestra) getting down and dirty with the folk.'
        }
      ],
      link: [
        { rel: 'preconnect', href: 'https://stats.g.doubleclick.net' },
        { rel: 'preconnect', href: 'https://www.googletagmanager.com' },
        { rel: 'preconnect', href: 'https://yt3.ggpht.com' },
        { rel: 'preconnect', href: 'https://fonts.gstatic.com' },
        { rel: 'preconnect', href: 'https://i.ytimg.com' },
        { rel: 'preconnect', href: 'https://www.google.com' },
        { rel: 'preconnect', href: 'https://www.google.co.uk' },
        { rel: 'preconnect', href: 'https://www.google-analytics.com' },
        { rel: 'preconnect', href: 'https://i.scdn.co' },
        { rel: 'preconnect', href: 'https://open.scdn.co' }
      ]
    }
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

.hero {
  background-image: url('~assets/images/dirty_boy_header.jpg');
  background-position: center;
  background-size: cover;
  /* height: 300px; */
  text-align: center;
  /* box-shadow: 0px 1px 5px 0px rgba(0, 0, 0, 0.75); */
  padding: 20px;
  background-color: #db8e3a;
  background-blend-mode: hard-light;
}

.hero__logo {
  width: 100%;
  max-width: 700px;
}
/* .hero__heading {
  color: white;
}

.hero__content {
  color: bisque;
} */
.main {
  /* background-color: hsl(12, 40%, 91%); */
  color: #3d4852;
  padding: 10px;
  max-width: 900px;
  margin: auto;
}

.main__media {
  padding-bottom: 20px;
}

.main__header {
  margin-bottom: 20px;
}

.main__heading {
  font-size: 20px;
  margin-top: 10px;
}

.main__paragraph {
  margin-bottom: 20px;
}

.link-list {
  padding-left: 0;
  list-style: none;
}

.link-list__item {
  font-size: 18px;
  line-height: 1.6;
}
.link-list__link,
.link-list__link:visited {
  color: rgb(0, 0, 238);
  text-decoration: none;
  font-weight: bold;
}

.media__header {
  margin-bottom: 10px;
}

.media__video {
  overflow: hidden;
  padding-bottom: 56.25%;
  position: relative;
  height: 0;
}
.media__video iframe {
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
  position: absolute;
}

@media (min-width: 475px) {
  /* .hero {
    height: 350px;
  } */
}
@media (min-width: 600px) {
  /* .hero {
    height: 400px;
  } */
}
@media (min-width: 750px) {
  /* .hero {
    height: 450px;
  } */
}
@media (min-width: 900px) {
  /* .hero {
    height: 600px;
  } */
}
@media (min-width: 1200px) {
  /* .hero {
    height: 650px;
  } */
}
</style>
