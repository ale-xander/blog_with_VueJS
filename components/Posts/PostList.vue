<template>
    <div class="posts-page">
    <section class="post-list">
    <PostPreview 
        id="1"
        :is-admin='isAdmin'
        thumbnail='https://images.unsplash.com/photo-1577457674844-da86606d2de6?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80'
        title='some turtles'
        previewText='my first post'
    />
    <PostPreview 
        id="2"
        :is-admin='isAdmin'
        thumbnail='https://images.unsplash.com/photo-1574923842719-94d5f9e28793?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1650&q=80'
        title='malo gato'
        previewText='a cat'
    />
    <PostPreview 
        id="3"
        :is-admin='isAdmin'
        thumbnail='https://images.unsplash.com/photo-1532022160153-7735cd049992?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2090&q=80'
        title='perro bueno'
        previewText='Dalmatian'
    />
    </section>
    </div>
</template>

<script>
  import PostPreview from '~/components/Posts/PostPreview'
  export default {
    components: {
      PostPreview
    },
    props: {
      isAdmin:{
        type: Boolean,
        default: false
      }
    }
  }
</script>



<style scoped>
.posts-page{
    display: flex;
    justify-content: center;
    align-items: center;
}
.post-list {
    display: flex;
    padding: 20px;
    box-sizing: border-box;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
}
</style>