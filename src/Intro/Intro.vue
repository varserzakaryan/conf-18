<template>
  <section class="Intro" id="Intro">
    <div class="Container">
      <div id="Titles">
        <h1 class="Title"><span>NodeConf</span> 2020 Armenia</h1>
        <span class="Title Subtitle">
          Apr <span>25</span>, 2020   -   <span>AUA</span>, Yerevan</span>
      </div>
      <!-- <a href="http://bit.ly/joinJSConf2018" class="Button -default" target="_blank">
        Request an Invite
      </a> -->
    </div>
  </section>
</template>

<script>
export default {

};
</script>

<style scoped lang="scss">
.Intro {
  display: flex;
  padding: 150px 0;
  align-items: center;
  justify-content: flex-start;
}

.Container {
  justify-content: center;
  display: flex;
}

.Title {
  font-family: Barlow;
  font-size: 70px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: center;
}

#Titles {
  display: inline-block;
}

.Subtitle {
  font-size: 24px;
  float: left;
}


@media (max-width: 800px) {
  .Title {
    font-size: 50px;
  }

  .Subtitle {
    font-size: 20px;
  }
}


@media (max-width: 700px) {
  .Title {
    font-size: 45px;
  }

  .Subtitle {
    font-size: 20px;
  }
}

@media (max-width: 600px) {
  .Button {
    padding: 0.7em 2em;
  }

  .Title {
    font-size: 40px;
  }

  .Subtitle {
    font-size: 20px;
  }
}

@media (max-width: 500px) {
  .Title {
    font-size: 35px;
  }

  .Subtitle {
    font-size: 20px;
  }
}

@media (max-width: 450px) {
  #Titles {
    display: grid;
  }
}

@media (max-height: 550px) {
  .Container {
    margin: -45px auto;
  }

  .Title {
    font-size: 40px;
  }
}

</style>
