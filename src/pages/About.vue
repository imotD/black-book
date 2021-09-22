<template>
  <Layout>
    <main>
      <header
        class="
          max-w-xl
          md:max-w-2xl
          xl:max-w-3xl
          mx-auto
          text-center
          px-6
          pt-24
        "
      >
        <h1 class="text-4xl sm:text-5xl md:text-6xl font-sans font-bold mb-1">
          About me
        </h1>
        <p class="text-grey-dark text-lg sm:text-3xl">Hanya Seonggok Pikiran</p>
      </header>
      <article
        class="
          max-w-xl
          md:max-w-2xl
          xl:max-w-3xl
          mx-auto
          px-6
          sm:px-12
          pt-16
          border-b border-gray-300
          pb-10
          mb-16
        "
      >
        <div class="markdown text-lg leading-normal text-gray-700">
          <p>
            Blog ini tercipta setelah nonton
            <span class="text-blue-500">The Social Network</span> di saat Mark
            Zuckerberg membuat blog untuk menceritakan kisahnya atau disebut
            <b><i>Diary</i></b>.
          </p>
        </div>
      </article>
      <site-footer class="pb-8 sm:pb-10" />
    </main>
  </Layout>
</template>

<script>
import config from "~/.temp/config.js";
import SiteFooter from "@/components/Footer";

export default {
  components: {
    SiteFooter,
  },
  metaInfo() {
    return {
      title: "About",
      meta: [
        {
          key: "description",
          name: "description",
          content: this.ogDescription,
        },

        { property: "og:type", content: "article" },
        { property: "og:title", content: "About" },
        { property: "og:description", content: this.ogDescription },
        { property: "og:url", content: `${this.config.siteUrl}/about/` },
        { property: "og:image", content: this.ogImageUrl },

        { name: "twitter:card", content: "summary_large_image" },
        { name: "twitter:title", content: "About" },
        { name: "twitter:description", content: this.ogDescription },
        { name: "twitter:site", content: "@cossssmin" },
        { name: "twitter:creator", content: "@cossssmin" },
        { name: "twitter:image", content: this.ogImageUrl },
      ],
    };
  },
  computed: {
    config() {
      return config;
    },
    ogDescription() {
      return "Introduction to the Bleda blog starter for Gridsome.";
    },
    ogImageUrl() {
      return `${this.config.siteUrl}/images/bleda-card.png`;
    },
  },
};
</script>
