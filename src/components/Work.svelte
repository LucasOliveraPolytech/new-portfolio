<script>
  import { fade } from 'svelte/transition';
  import YouTube from 'svelte-youtube'
  export let header
  export let body
  export let media
  export let outLink
  export let mediaWidth = '65%'

  const options = {
    height: '390',
    width: '640',
    //  see https://developers.google.com/youtube/player_parameters
    playerVars: {
      autoplay: 1
    }
  };

  function onReady(event) {
    // access to player in all event handlers via event.target
    event.target.pauseVideo();
  }
</script>

<div
  class='work'
  style='--media-width: {mediaWidth}'
  in:fade={{delay: 300, duration: 500}} out:fade>
  <div class='media'>
    <YouTube videoId="BAYw_orzBR0" />
    <!-- <img src={media} alt={header} /> -->
  </div>
  <div class='text-container'>
    <div class='text'>
      <h2>{header}</h2>
      {@html body}
      {#if outLink}
        <p>
          <a href={outLink} target="_blank">Check it out!</a>
        </p>
      {/if}
    </div>
  </div>
</div>

<style>
  img {
    width: 100%;
  }

  a {
    color: red;
  }

  .work {
    display: flex;
    flex-direction: row;
    align-items: center;
    flex: 1;
    box-sizing: border-box;
    width: 100%;
    padding: 20px 0;
  }

  .media {
    min-width: var(--media-width);
    box-sizing: border-box;
    padding: 20px;
    border-right: 1px solid black;
    display: flex;
    flex: 1;
    justify-content: center;
    align-items: center;
  }

  img {
    object-fit: contain;
    flex: 1;
    max-height: 100%;
  }

  .text-container {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: scroll;
  }

  .text {
    margin: auto;
    padding: 20px;
  }

  @media only screen and (max-width: 1000px) {
    .work {
      flex-direction: column;
    }

    .text-container {
      overflow: visible;
    }

    .text {
      min-height: 100%;
    }

    .media {
      border-bottom: 1px solid black;
      border-right: none;
    }
  }
</style>
