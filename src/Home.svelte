<script>
  import { fade } from 'svelte/transition'
  import Work from './components/Work.svelte'
  const link = "<a href='https://catalyticsound.com/''>Catalytic Sound</a>"
  const me = {
    title: "AgileTalk",
    description: "<p>This is a product of Agile Bots Synthetics Corp, a fictional company created for such product.</p>",
    media: {
      videoId: "BAYw_orzBR0"
    }
  }
</script>

<Work
  header={me.title}
  body={me.description}
  media={me.media} />

<style>
  .bio {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 0 100px;
  }

  a {
    color: red;
  }

</style>
