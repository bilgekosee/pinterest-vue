<template>
  <v-container>
    <div></div>
    <stack :column-min-width="320" :gutter-width="10" :gutter-height="8">
      <stack-item v-for="(item, i) in items" :key="i">
        <image-card
          :url="item.url"
          :meta="{
            name: item.name,
            occupation: item.occupation,
            profileImageUrl: item.profileImageUrl,
          }"
        />
      </stack-item>
    </stack>
  </v-container>
</template>

<script>
import { Stack, StackItem } from "vue-stack-grid";
import ImageCard from "../components/ImageCard";

export default {
  components: { Stack, StackItem, ImageCard },
  data() {
    return {
      items: [
        {
          url: "https://images.unsplash.com/photo-1492571350019-22de08371fd3?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTB8fGphcGFufGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60",
          name: "Torii Gate",
          occupation: "Photographer",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1276567411240681472/8KdXHFdK_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1524413840807-0c3cb6fa808d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTJ8fGphcGFufGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60",
          name: "canal between cherry blossom trees",
          occupation: "Doctor",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1609568387507666944/dgldUz8g_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1509023464722-18d996393ca8?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTZ8fGphcGFufGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60",
          name: "fuji mountain",
          occupation: "geologist",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1512723839595204611/z8DaGRfm_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1491884662610-dfcd28f30cfb?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTd8fGphcGFufGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60",

          name: "himeji castle",
          occupation: "teacher",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1602748422393663488/8Haxj1CG_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1557409518-691ebcd96038?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mjl8fGphcGFufGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60",
          name: "boats on body of water",
          occupation: "photographer",
          profileImageUrl:
            "https://images.unsplash.com/profile-1589679453430-2c3a0da4a34fimage?dpr=1&auto=format&fit=crop&w=150&h=150&q=60&crop=faces&bg=fff",
        },
        {
          url: "https://images.unsplash.com/photo-1478436127897-769e1b3f0f36?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MzB8fGphcGFufGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60",

          name: "red and black wooden pillar",
          occupation: "student",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1548895704944361473/JmZja60Z_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1515666991427-9b0f67becfa1?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mjd8fGJvb2slMjBhbmQlMjBjb2ZmZXxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60",

          name: "book",
          occupation: "literary man",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/483545268139597824/-y692bMn_400x400.jpeg",
        },
        {
          url: "https://images.unsplash.com/photo-1628251765667-7f23da5766e5?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1064&q=80",

          name: "book and coffee",
          occupation: "photographer",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1530182186091044866/1Mw6JG9k_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1528731918315-d95040a988ba?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Nzh8fGJvb2slMjBhbmQlMjBjb2ZmZXxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60",

          name: "starbucks",
          occupation: "waiter",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1525924474876571648/88afEaYk_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1553877522-43269d4ea984?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80",

          name: "coffee",
          occupation: "barista",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1474867465226264580/UTtELJWE_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1519389950473-47ba0277781c?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTV8fHNvZnR3YXJlfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60",

          name: "software",
          occupation: "developer",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1629902582813532161/a4at9rm0_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1581090464777-f3220bbe1b8b?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NTF8fHNvZnR3YXJlfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60",

          name: "robotic",
          occupation: "engineer",
          profileImageUrl:
            "https://pbs.twimg.com/profile_images/1564398871996174336/M-hffw5a_400x400.jpg",
        },
        {
          url: "https://images.unsplash.com/photo-1567449303183-ae0d6ed1498e?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Njl8fHNvZnR3YXJlfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60",

          name: "building",
          occupation: "civil engineer",
          profileImageUrl:
            "https://avatars.githubusercontent.com/u/68377756?v=4",
        },
        {
          url: "https://images.unsplash.com/photo-1533929702053-9986939ea193?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=735&q=80",
          name: "life",
          occupation: "singer",
          profileImageUrl:
            "https://images.unsplash.com/profile-fb-1498159596-9b7375a4c15c.jpg?dpr=1&auto=format&fit=crop&w=150&h=150&q=60&crop=faces&bg=fff",
        },
      ],
    };
  },
};
</script>

<style>
</style>