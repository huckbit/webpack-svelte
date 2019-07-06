<script>
  let data = {
    message: "Svelte webpack it's working",
    url: [
      "https://svelte.dev/",
      "https://github.com/huckbit/webpack-svelte.git"
    ],
    image:
      "https://raw.githubusercontent.com/sveltejs/svelte/29052aba7d0b78316d3a52aef1d7ddd54fe6ca84/site/static/images/svelte-android-chrome-512.png",
    imageName: "svelte-logo"
  };
</script>

<style>
  .container {
    padding: 15px;
    color: #ff3e00;
    font-family: sans-serif;
  }
  a {
    color: #ff3e00;
  }
  .xy-center {
    height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
</style>

<div class="container xy-center">
  <a href={data.url[0]} target="_blank">
    <img src={data.image} alt={data.imageName} height="250" />
  </a>
  <h1 class="text-color">{data.message}!</h1>
  <a href={data.url[1]}>{data.url[1]}</a>
</div>
