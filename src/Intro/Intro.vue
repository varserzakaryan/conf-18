<template>
  <section class="Intro" id="Intro">
    <div class="Container">
      <h1 class="Title">JavaScript Conference <br> Armenia</h1>
      <h3 class="Subtitle">November 3, 2018</h3>
      <a href="" class="Button -default">
        Request an Invite
      </a>
    </div>

    <div class="IntroSponsor">
      <div>
        <a href="https://www.simplytechnologies.net/" target="_blank">
          <img src="/sponsors/simply.svg" width="320" />
        </a>
      </div>
      <div class="Description">
        Main sponsor
      </div>
    </div>

    <div class="IntroBgMain"></div>
    <div class="IntroBgLeft"></div>
    <div class="IntroBgRight"></div>
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

.IntroSponsor {
  position: absolute;
  right: 5%;
  bottom: 30px;
  display: block;
  font-size: .8em;
  text-align: center;
}

.IntroBgLeft {
  position: absolute;
  left: 0;
  top: 0;
  width: 50%;
  height: 100%;
  background-image: url('./IntroBgLeft.svg');
  background-repeat: no-repeat;
  background-size: contain;
  z-index: -1;
}

.IntroBgMain {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-image: url('./IntroBgMain.png');
  background-repeat: no-repeat;
  background-size: 60vh;
  background-position-y: 65%;
  background-position-x: center;
  z-index: -1;
}

.IntroBgRight {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  z-index: -1;

  &:after {
    position: absolute;
    left: 65%;
    top: 15%;
    width: 30vh;
    height: 30vh;
    border-radius: 50%;
    background-color: #ffdd00;
    display: block;
    content: " ";
  }
}
</style>
