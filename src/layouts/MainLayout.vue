<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="transparent">
      <q-toolbar class="flex big-height" ref="qtb">
        <q-avatar rounded>
          <img src="~/assets/icon.png" />
        </q-avatar>

        <q-toolbar-title>
          TecnicoCelulares
        </q-toolbar-title>

        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="leftDrawerOpen = !leftDrawerOpen"
        />
      </q-toolbar>
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      bordered
      content-class=""
      overlay
      right
      dark
      class="transparent"
    >
      <q-list>
        <q-item-label header>
          Essential Links
        </q-item-label>
        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>

      <q-img class="absolute-top" src="~/assets/icon.png" style="height: 150px">
        <div class="absolute-bottom bg-transparent">
          <q-avatar size="56px" class="q-mb-sm">
            <img src="https://cdn.quasar.dev/img/boy-avatar.png" />
          </q-avatar>
          <div class="text-h5 text-weight-bold">Facundo Lopez</div>
          <div>MLUSER</div>
        </div>
      </q-img>
    </q-drawer>

    <q-page-container>
      <router-view />
      <q-scroll-observer @scroll="onScroll" />
    </q-page-container>
  </q-layout>
</template>

<script>
import EssentialLink from "components/EssentialLink.vue";

const linksData = [
  {
    title: "Docs",
    caption: "quasar.dev",
    icon: "school",
    link: "https://quasar.dev"
  },
  {
    title: "Github",
    caption: "github.com/quasarframework",
    icon: "code",
    link: "https://github.com/quasarframework"
  },
  {
    title: "Discord Chat Channel",
    caption: "chat.quasar.dev",
    icon: "chat",
    link: "https://chat.quasar.dev"
  },
  {
    title: "Forum",
    caption: "forum.quasar.dev",
    icon: "record_voice_over",
    link: "https://forum.quasar.dev"
  },
  {
    title: "Twitter",
    caption: "@quasarframework",
    icon: "rss_feed",
    link: "https://twitter.quasar.dev"
  },
  {
    title: "Facebook",
    caption: "@QuasarFramework",
    icon: "public",
    link: "https://facebook.quasar.dev"
  },
  {
    title: "Quasar Awesome",
    caption: "Community Quasar projects",
    icon: "favorite",
    link: "https://awesome.quasar.dev"
  }
];

export default {
  name: "MainLayout",
  components: { EssentialLink },
  data() {
    return {
      leftDrawerOpen: false,
      essentialLinks: linksData
    };
  },

  methods: {
    onScroll(info) {
      if (info.position > 100) {
        this.$refs.qtb.$el.classList.remove("big-height");
        this.$refs.qtb.$el.classList.add("bg-darken");
      } else {
        this.$refs.qtb.$el.classList.add("big-height");
        this.$refs.qtb.$el.classList.remove("bg-darken");
      }
    }
  }
};
</script>
<style lang="scss" scoped>
.big-height {
  background: rgba(0, 0, 0, 1); /* fallback for old browsers */
}
.bg-darken {
  background-color: rgba(0, 0, 0, 0.5);
}
.q-toolbar {
  transition: background-color 0.5s ease-out;
}
@media screen and (min-width: 960px) {
  .q-toolbar {
    padding-left: 150px;
    padding-right: 150px;
  }
}
</style>
