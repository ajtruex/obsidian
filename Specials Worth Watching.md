website with all the stand up specials I find good and worth watching

New York Comics

LA Comics

Podcasts of each comedian


- Bill Burr Live at Red Rocks
https://www.netflix.com/us/title/81457341?s=i&trkid=13747225&vlang=en&clip=81618230

![](9A9AED59-F679-42AF-B2FC-DEEA762D7EE8.jpeg)

![](969A684D-1AB4-44EE-B22F-39CB1D4A955E.jpeg)

![](DE256C7D-7E77-45DB-A785-0A63E1FA60F8.jpeg)
![](MacBook%20Pro%2016_%20-%201%201.png)

API Request
https://api.themoviedb.org/3/movie/982679?api_key=6c3a605f23df401b0f1a36baa263c71a&language=en-US

YouTube API
```
<!DOCTYPE html>
<html>
  <body>
    <!-- 1. The <iframe> (and video player) will replace this <div> tag. -->
    <div id="player"></div>

    <script>
      // 2. This code loads the IFrame Player API code asynchronously.
      var tag = document.createElement('script');

      tag.src = "https://www.youtube.com/iframe_api";
      var firstScriptTag = document.getElementsByTagName('script')[0];
      firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);

      // 3. This function creates an <iframe> (and YouTube player)
      //    after the API code downloads.
      var player;
      function onYouTubeIframeAPIReady() {
        player = new YT.Player('player', {
          height: '390',
          width: '640',
          videoId: 'M7lc1UVf-VE',
          playerVars: {
            'playsinline': 1
          },
          events: {
            'onReady': onPlayerReady,
            'onStateChange': onPlayerStateChange
          }
        });
      }

      // 4. The API will call this function when the video player is ready.
      function onPlayerReady(event) {
        event.target.playVideo();
      }

      // 5. The API calls this function when the player's state changes.
      //    The function indicates that when playing a video (state=1),
      //    the player should play for six seconds and then stop.
      var done = false;
      function onPlayerStateChange(event) {
        if (event.data == YT.PlayerState.PLAYING && !done) {
          setTimeout(stopVideo, 6000);
          done = true;
        }
      }
      function stopVideo() {
        player.stopVideo();
      }
    </script>
  </body>
</html>
```

Convert Figma desgin to actual website
Figure out whether to use Vue.js, React, or Next

