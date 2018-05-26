<template>
    <div class="theme-container">
        <div class="content">
            <h1>404</h1>
            <blockquote>{{ getMsg() }}</blockquote>
            <router-link to="/">Take me home.</router-link>
        </div>
    </div>
</template>

<script>
const msgs = [
  `Aww There's nothing here.`,
  `Aww How did we get here?`,
  `Aww That's a Four-Oh-Four.`,
  `Aww Looks like we've got some broken links.`
];

export default {
  methods: {
    getMsg() {
      return msgs[Math.floor(Math.random() * msgs.length)];
    }
  }
};
</script>
