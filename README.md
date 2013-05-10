### Basic Usage
```javascript
$(document).ready(function(){
  var api;
  var mysongs = [
    {
      "url": "sound/1.mp3",
      "artist": "Artist1",
      "title": "Song1",
      "thumb":"images/1.jpg",
      "custom": "myCustomData1"  
    }
    ,
    {
      "url": "sound/2.mp3",
      "artist": "Artist2",
      "title": "Song2",
      "thumb": "images/2.jpg",
      "custom": "myCostomData2"
    }
  ];

  $('#swagg-player').SwaggPlayer({
    data: mysongs
  });
});
```
### Params

| **Param**     | **Type**         | **default**     | **Description** |
| :------------ | :--------------  | :-------------- | :-------------- |
| data          | JSON Array       | n/a            | Song configuration |
| buttonHover   | boolean          | false          | Change button on button hover 
| eagerLoad     | boolean          | false          | Loads songs immediately on page load |
| autoPlay      | boolean          | false          | Starts playing the first song when the player finishes initializing |
| whilePlaying  | function         | null           | Fires at a regular interval while a sound is playing |
| onStop        | function         | null           | Fires when the music is stopeed |
| onSeekPreview | function         | null           | Fires when someone hovers over the progress bar |
| onSetupComplete | function       | null           | Fires when the player finishes initializing |
| whileLoading  | function         | null           | Fires regularly while a song is loading |
| onPlay        | function         | null           | Fires when a song starts playing |
| onPause       | function         | null           | Fires when a song is paused |

See index.html for markup and API examples. 
Go to http://johnnyray.me for a demo. Feel free to reach out if you have any questions.


