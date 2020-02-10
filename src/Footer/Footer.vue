<template>
  <div class="Footer">

    <div class="LogoContainer">
      <a href="#Intro" class="LogoLink">
        <Logo
          :size="150" />
      </a>
    </div>

    <div class="SocialLinks">
      <a class="SocialIcon Icon-Github" href="https://github.com/JSConfArmenia/" target="_blank"></a>
      <a class="SocialIcon Icon-Facebook" href="https://www.facebook.com/jsconf.am/" target="_blank"></a>
      <a class="SocialIcon Icon-Twitter" href="https://twitter.com/jsconf_am/" target="_blank"></a>
      <a class="SocialIcon Icon-Instagram" href="https://www.instagram.com/jsconf.am/" target="_blank"></a>
      <a class="SocialIcon Icon-Youtube" href="https://www.youtube.com/channel/UCkzEOKU959F6_T0OaQBH4VQ/featured" target="_blank"></a>
    </div>

    <div class="PressRelease">
      Press Release
      <a href="/Press-Release-EN.pdf" target="_blank">En</a> |
      <a href="/Press-Release-AM.pdf" class="AM" target="_blank">Am</a>
    </div>

    <p class="Credits">
      Design and branding by
      <a href="http://digitalfactory.co/" target="_blank">Digital Factory</a>,
      coded in Vue.js by <a class="Devs" href="https://github.com/nairihar" target="_blank">@nairihar</a>,
      <a class="Devs" href="https://github.com/tovmassian" target="_blank">@tovmassian</a> and
      <a class="Devs" href="https://github.com/NodeJSArmenia/conf-20/graphs/contributors" target="_blank">others</a>.
    </p>
  </div>
</template>

<script>
import Logo from '../_common/Logo/Logo.vue';

export default {
  components: {
    Logo,
  },
};
</script>

<style scoped lang="scss">
.Footer {
  min-height: 350px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  flex-direction: column;
  position: relative;
  padding-bottom: 50px;
}

.LogoContainer {
  margin: 20px 0;
}

.SocialLinks {
  display: flex;
  margin-bottom: 15px;
}

.PressRelease {
  font-family: Barlow;
  font-size: 20px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.25;
  letter-spacing: 0.5px;

  a {
    color: #6cc24a;
    text-transform: uppercase;
  }

  .AM {
    color: white;
  }
}

.SocialIcon {
  background: center;
  width: 32px;
  height: 32px;
  margin: 3px;
  padding: 5px;
  background-repeat: no-repeat;
  background-size: 20px;
  background-position: center;
  display: block;
  position: relative;
  overflow: hidden;

  &:after {
    content: " ";
    display: block;
    background-color: #91919145;
    position: absolute;
    transition: all .2s ease;
    top: 100%;
    left: 0;
    width: 100%;
    height: 100%;
  }

  &.active,
  &:hover {
    &:after {
      top: 0;
    }
  }
}

.Icon-Github {
  background-image: url('./github.png');
}

.Icon-Twitter {
  background-image: url('./twitter.png');
}

.Icon-Facebook {
  background-image: url('./facebook.png');
  background-size: 12px;
}

.Icon-Instagram {
  background-image: url('./instagram.png');
}

.Icon-Youtube {
  background-image: url('./youtube.png');
}

.Credits {
  margin: 20px;
  font-family: Barlow;
  font-size: 20px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.25;
  letter-spacing: 0.5px;

  a {
    color: #6cc24a;
  }

  .Devs {
    color: #fff;
  }
}

a:not(.LogoLink):not(.SocialIcon) {
  text-decoration: underline;
  font-weight: bold;
}

@media (max-width: 500px) {
  .Footer {
    min-height: 500px;
  }
}

</style>
