<template>
  <main class="card">
    <div class="card-header">
      <img :src="user.avatar" :alt="`Portrait of ${user.name}`" />
      <h1 class="text-preset-1">{{ user.name }}</h1>
      <p class="text-preset-2-bold text-color-green">{{ user.address }}</p>
      <p class="text-preset-2 card-header__job">{{ user.job }}</p>
    </div>
    <div class="card-links" aria-label="Social profiles">
      <ul>
        <li v-for="link in socialLinks" :key="link.id">
          <a
            class="text-preset-2-bold"
            :href="link.source"
            target="_blank"
            rel="noopener noreferrer"
            >{{ link.label }}</a
          >
        </li>
      </ul>
    </div>
  </main>
</template>
<script setup>
import avatarJessica from "../assets/avatar-jessica.jpeg";

const user = {
  avatar: avatarJessica,
  name: "Jessica Randall",
  address: "London, United Kingdom",
  job: '"Front-end developer and avid reader."',
};
const socialLinks = [
  {
    id: 0,
    label: "GitHub",
    source: "https://github.com/",
  },
  {
    id: 1,
    label: "Frontend Mentor",
    source: "https://www.frontendmentor.io/",
  },
  {
    id: 2,
    label: "LinkedIn",
    source: "https://www.linkedin.com/",
  },
  {
    id: 3,
    label: "Twitter",
    source: "https://x.com/",
  },
  {
    id: 4,
    label: "Instagram",
    source: "https://www.instagram.com/",
  },
];
</script>
<style lang="css" scoped>
.card {
  box-sizing: border-box;
  width: min(384px, 100%);
  padding: 40px;
  background-color: var(--color-grey-800);
  border-radius: 12px;
  @media screen and (max-width: 425px) {
    padding: 24px;
  }
  .card-header {
    text-align: center;
    img {
      width: 88px;
      height: 88px;
      border-radius: 100%;
      margin-bottom: 24px;
    }
    .card-header__job {
      margin-top: 24px;
    }
  }
  .card-links {
    margin-top: 24px;
    ul {
      list-style: none;
      li + li {
        margin-top: 16px;
      }
      a {
        display: block;
        padding: 12px;
        border-radius: 8px;
        text-align: center;
        text-decoration: none;

        background-color: var(--color-grey-700);
        color: var(--color-white);

        &:hover {
          background-color: var(--color-green);
          color: var(--color-grey-900);
        }

        &:focus-visible {
          outline: 2px solid var(--color-green);
          outline-offset: 3px;
        }
      }
    }
  }
}
</style>
