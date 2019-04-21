<template>
  <div>
    <header class="hero">
      <h1 class="hero__heading">Portland Brothers</h1>
      <p class="hero__content">Old friends; new songs.</p>
    </header>
    <main class="main">
      <h6 class="main__heading">The brothers</h6>
      <!-- <p class="main__paragraph">
        Steven Adams and Timothy Victor first met in the summer of 2001 at The
        Portland Arms, Cambridge. Adams had just put together The Broken Family
        Band, who would go on to be one of the best-loved cult bands to come out
        of the city, whilst TV was playing in Chris T-T’s band and fronting his
        own, sprawling ‘country and eastern’ outfit The Folk Orchestra.
      </p>

      <p class="main__paragraph">
        Over the next few years the two became firm friends, with Victor
        producing the first two Broken Family Band albums and performing live
        with the group as the unofficial ‘fifth member’. They also collaborated
        on the 2005 album ‘Problems’, played a few sweaty London club shows with
        a short-lived rock band, and sang together as part of an unaccompanied
        vocal group, wearing false beards.
      </p>

      <p class="main__paragraph">
        Since The Broken Family Band split in 2009, Adams has continued to
        perform and record, releasing two albums with breezy indie-rock outfit
        Singing Adams, and two solo records as well as last year’s
        politically-charged Virtue Signals (as Steven Adams & The French Drops).
        TV continued to perform with The Folk Orchestra, as well as writing
        music for television and doing ‘something with computers’.
      </p>

      <p class="main__paragraph">
        Adams says: “When we first met, TV lived in London and I lived in
        Cambridge. A couple of years later I moved to London and he now lives in
        Cambridge. I don’t know if this means anything”.
      </p>

      <p class="main__paragraph">
        TV says: “My band played Steve’s birthday party at his house last year,
        and we sang together for the first time in ages. That was when we
        realised we should make some music together.”
      </p>-->

      <p class="main__paragraph">
        Steven Adams and Timothy Victor first met in the summer of 2001 at The
        Portland Arms, Cambridge. They got involved.
      </p>
      <p class="main__paragraph">
        Portland Brothers sees the duo returning to the music that first brought
        them together; writing and singing songs that reflect their shared love
        of folk music, country rock and classic disco. They’re currently writing
        and recording for an album due for release later in 2019.
      </p>
      <ul class="link-list">
        <li class="link-list__item">
          <a
            class="link-list__link"
            href="https://portlandbrothers.bandcamp.com/"
            >Go and get our music</a
          >
        </li>
        <li class="link-list__item">
          <a class="link-list__link" href="https://twitter.com/portbros"
            >Twitter: @portbros</a
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
  background-image: url('~assets/images/IMG_0011-2.jpg');
  background-position: center;
  background-size: cover;
  height: 300px;
  text-align: center;
  box-shadow: 0px 1px 5px 0px rgba(0, 0, 0, 0.75);
}
.hero__heading {
  color: white;
}

.hero__content {
  color: bisque;
}
.main {
  /* background-color: hsl(12, 40%, 91%); */
  color: #3d4852;
  padding: 10px;
}
.main__heading {
  font-size: 20px;
  margin-top: 10px;
  margin-bottom: 20px;
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

@media (min-width: 475px) {
  .hero {
    height: 350px;
  }
}
@media (min-width: 600px) {
  .hero {
    height: 400px;
  }
}
@media (min-width: 750px) {
  .hero {
    height: 450px;
  }
}
@media (min-width: 900px) {
  .hero {
    height: 600px;
  }
}
@media (min-width: 1200px) {
  .hero {
    height: 650px;
  }
}
</style>
