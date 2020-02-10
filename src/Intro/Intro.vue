<template>
  <section class="Intro" id="Intro">
    <div class="Container">
      <h1 class="Title">NodeConf 2020<br> Armenia</h1>
      <h3 class="Subtitle">April 25, 2020</h3>
      <a href="http://bit.ly/joinJSConf2018" class="Button -default" target="_blank">
        Request an Invite
      </a>
    </div>
  </section>
</template>

<script>
export default {

};
</script>

<style scoped lang="scss">
.Intro {
  min-height: 100vh;
  display: flex;
  padding: 150px 0;
  align-items: center;
  justify-content: flex-start;
}

.Title {
  font-size: 60px;
  line-height: 70px;
  font-weight: 900;
  text-transform: none;
}

.Subtitle {
  font-size: 36px;
}

@media (max-width: 450px) {
  .Subtitle {
    text-shadow: 1px 1px 1px #f5f5f591;
  }
}

@media (max-width: 700px) {
  .Title {
    font-size: 45px;
  }

  .Subtitle {
    font-size: 30px;
  }
}

@media (max-width: 600px) {
  .Button {
    padding: 0.7em 2em;
  }

  .Title {
    line-height: 55px;
  }

  .Subtitle {
    font-size: 27px;
  }
}

@media (max-height: 550px) {
  .Container {
    margin: -45px auto;
  }

  .Title {
    line-height: 55px;
    font-size: 40px;
  }
}

</style>
