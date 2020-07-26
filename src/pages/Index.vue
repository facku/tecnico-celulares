<template>
  <q-page>
    <div class="section-1 row">
      <div class="texto col-12 col-md-6 flex content-center">
        <div class="title">TECNICO CELULARES</div>
        <p class="description">
          Asistente Virtual para locales de
          <span>Reparacion y Venta de accesorios</span>
          para telefonos celulares integrado con MercadoLibre.<br />Gestiona tus
          clientes y presupuestos de forma mas facil.
        </p>
      </div>
      <div class="col-12 col-md-6 q-px-xl">
        <img src="~assets/Product-teardown-amico.svg" class="fit" />
      </div>
    </div>

    <div class="relative-position">
      <div class="custom-shape-divider-bottom-1595652012">
        <svg
          data-name="Layer 1"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 1200 120"
          preserveAspectRatio="none"
        >
          <path
            d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z"
            opacity=".25"
            class="shape-fill"
          ></path>
          <path
            d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z"
            opacity=".5"
            class="shape-fill"
          ></path>
          <path
            d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z"
            class="shape-fill"
          ></path>
        </svg>
      </div>
    </div>

    <div class="row bg-purple-2" style="margin-top:-2px">
      <div class="col-12 col-md-6">
        <img src="~assets/Product-teardown-bro.svg" class="full-width" />
      </div>
      <div class="texto col-12 col-md-6 flex content-center">
        <div class="subtitle">TECNICO CELULARES</div>
        <p class="subdescription">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio
          recusandae voluptatem ipsam provident temporibus. Lorem ipsum, dolor
          sit amet consectetur adipisicing elit. Quas debitis dolorem nisi alias
          illo exercitationem deserunt atque aliquam nam? Ratione amet assumenda
          soluta ad! Quos.<br /><br />
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio
          recusandae voluptatem ipsam provident temporibus. Lorem ipsum, dolor
          sit amet consectetur adipisicing elit. Quas debitis dolorem nisi alias
          illo exercitationem deserunt atque aliquam nam? Ratione amet assumenda
          soluta ad! Quos.
        </p>
      </div>
    </div>

    <div class="section-3 row bg-purple-8">
      <div class="texto col-12 col-md-6 flex content-center">
        <div class="subtitle ">TECNICO CELULARES</div>
        <div class="description ">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio
          recusandae voluptatem ipsam provident temporibus. Lorem ipsum dolor
          sit amet consectetur adipisicing elit.
        </div>
      </div>
      <div class="img-container col-12 col-md-6 self-center">
        <img src="~assets/Product-teardown-pana.svg" class="full-width" />
      </div>
    </div>
  </q-page>
</template>

<script>
export default {
  name: "PageIndex"
};
</script>
<style lang="scss" scoped>
.row {
  overflow: hidden;
  .texto {
    color: white;
    padding: 0 1em;
  }

  .title {
    font-size: 2.2rem;
    font-weight: 900;
    text-shadow: 1rem 0.1rem 2rem rgb(255, 0, 242),
      0rem 0.2rem 2rem rgb(250, 29, 0);
  }

  .subtitle {
    font-size: 2.2rem;
    font-weight: 700;
    text-shadow: 1rem 0.1rem 1rem rgb(255, 0, 242),
      0rem 0.2rem 1.2rem rgb(250, 29, 0);
  }

  .description {
    font-size: 1.5rem;
    font-weight: 200;

    text-shadow: 1rem 0.1rem 1rem rgb(255, 0, 242),
      0rem 0.2rem 1.2rem rgb(250, 29, 0);

    & span {
      font-weight: 700;
    }
  }

  .subdescription {
    font-size: 1.2rem;
    font-weight: 300;
    background: rgb(168, 6, 197);
    padding: 1.5rem 3rem;
    border-radius: 8px;
  }
}

@media screen and (max-width: 600px) {
  .row {
    padding-bottom: 5rem;
    .texto {
      order: 1;
    }
  }
  .section-1 {
    padding-bottom: 10rem;
  }
}

@media screen and (min-width: 767px) {
  .row {
    min-height: 100vh;
    .subtitle {
      font-size: 3rem;
      font-weight: 700;
    }

    .description {
      font-size: 1.5rem;
      font-weight: 200;
    }

    .subdescription {
      font-size: 1rem;
      font-weight: 300;
    }
    .title {
      font-size: 5rem;
      line-height: 5rem;
      order: 0;
    }
  }

  .section-1 {
    text-align: right;
  }

  /* Section 3 */
  .section-3 {
    position: relative;
    .img-container,
    .texto {
      z-index: 1;
    }
    &::after {
      content: "";
      position: absolute;
      z-index: 0;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: $purple-6;
      clip-path: circle(75% at 100% 100%);
    }
  }
}

.section-1 {
  background: url("~assets/bg/Liquid-Cheese.svg");
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment: fixed;
}

/* Waves separator */
.custom-shape-divider-bottom-1595652012 {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
  transform: rotate(180deg);
}

.custom-shape-divider-bottom-1595652012 svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 81px;
}

.custom-shape-divider-bottom-1595652012 .shape-fill {
  fill: #e1bee7;
}

/* Animations */
.section-1 img {
  animation: intro-right 0.4s 1.5s cubic-bezier(0.23, 1, 0.32, 1) backwards;
}

.section-1 .texto {
  animation: intro-left 0.7s 2.1s cubic-bezier(0.23, 1, 0.32, 1) backwards;
}

@keyframes intro-right {
  0% {
    opacity: 0;
    transform: translateX(200px);
  }
  50% {
    opacity: 0.2;
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes intro-left {
  0% {
    opacity: 0;
    transform: translateX(-200px);
  }
  50% {
    opacity: 0.2;
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}
</style>
