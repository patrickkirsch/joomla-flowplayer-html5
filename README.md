joomla-flowplayerr-html5
========================

Joomla plugin for Flowplayer, with browser capability checks

The major code originates from FlowPlayer Reloaded by tushev.org.

This extends the plugin for browser checking and selecting the appropriate video file.
E.g.:
        - if Flash is available take flash 
        - if MP4 is available (html5 <video>, e.g. Apple*) prefer this.
        - if ogg is available (html5 <video>, e.g. Firefox) prefer this.

So this code should now work with every browser (Apple, Opera, Firefox), even on mobile.

<b>Furthermore RTMP is now understood.</b>

Hint: this needs a seperate streaming server.

<h3>An example:</h3>
Implement this in your Joomla page editor.
<pre>
{flowplayer popup=1 width=90 height=90
        img=/images/girlsteam_sachsen_team_v04.jpg
        mpfour=images/videos/girlsteam_sachsen_sport_im_osten_20140413.mp4
        webm=images/videos/girlsteam_sachsen_sport_im_osten_20140413.webm}
        rtmp://ww8.olanis.net/flvplayback/mp4:girlsteam_sachsen_sport_im_osten_20140413_1280x720.mp4
{/flowplayer}
</pre>

<h3>Installation</h3>
Just download <pre>plg_FlowPlayer.Reloaded-3.1_j16-multiplatform-pk.zip</pre> and install it as Joomla plugin.

