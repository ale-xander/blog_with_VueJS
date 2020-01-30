<template>
<div class="home-page">
  <section class="intro">
    <h1>some headline for front page</h1>
  </section>
  <section class="featured-posts">
    <nuxt-link :to="  '/posts/'+1 " class="post-preview">
      <article >
        <div class="post-thumbnail" style="background-image: url(https://images.unsplash.com/photo-1577457674844-da86606d2de6?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80)"></div>
        <div class="post-content">
          <h1>Post title</h1>
          <p>some preview text</p>
        </div>
      </article>
    </nuxt-link>
    <nuxt-link :to="  '/posts/'+2 " class="post-preview">
      <article >
        <div class="post-thumbnail" style="background-image: url(https://images.unsplash.com/photo-1572880393162-0518ac760495?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1267&q=80)"></div>
        <div class="post-content">
          <h1>Post title two</h1>
          <p>some preview text two</p>
        </div>
      </article>
    </nuxt-link>
  </section>

</div>
</template>

<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

.post-preview {
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #ccc;
  background-color: white;
  width: 90%;
}

a {
  text-decoration: none;
  color: black;
}

@media (min-width: 850px) {
  .post-preview {
    width: 400px;
    margin: 10px;
  }
}

.post-thumbnail {
  width: 100%;
  height: 200px;
  background-position: center;
  background-size: cover;
}

.post-content {
  padding: 10px;
  text-align: center;
}

a:hover .post-content,
a:active .post-content {
  background-color: #ccc;
}
</style>