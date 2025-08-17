# HTML and JS based local MP4-video player, by Dr. ChenGuang
## Click the button and select an mp4 file, it will be played. Move mouse closed to the bottom of the video area, controlers will appear.
- Double click on the video to show in full-screen, Esc-key to exit full-screen.
- Single-click on the video to pause/play. From 030 on, right-click on the video to pause/play.
- Drag with left-mouse-button to move the video.
- Mouse-wheel to jump forward or backward in time.
- Mouse-wheel with left-mouse-button held to rotate the video.
- Mouse-wheel with right-mouse-button held to zoom the video.
- Click mouse-wheel to fit the video to the screen-height.
## From 027 on, added auto-hide buttons for jumping to the specified time-locations:
- Move mouse to the upper-left coner, a button appears. Click the button and select an MP4 file in local disk. 
- This softwear automatically finds out all the contents like "Get up 0H12M5S, go to school 1H5M27S, lunch 6H20M50S.mp4", 
- and generates buttons like "Get up 0H12M5S" , "go to school 1H5M27S" , "lunch 6H20M50S". 
- The buttons appears when mouse is closed to the left side. Click the button, jumps to the related time in the video.
## From 028 on, added timeDisplayer and optimized div-div based dom-location-control:
- Added a timeDisplayer to display the time of video. 
- Click on the timeDisplayer to copy the time-string in it. 
- Optimized div-div based dom-location-control.
## From 037 on, Added text-input-area at the top to help writing title-time: 
- When mouse is near the top, it appears. 
- Choose an mp4 file, the file-name appears in the text-input-area. 
- Right-click the text-input area, the present video-time like 1H23M7S is automatically added to the end of the text, 
- The insert cursor is placed at the proper place for typing a title for the video-time. 
- Press Enter-key, the text will be copied into clip-board and saved into LocalStorage of your Browser. 
- You can rename the mp4 file with the text in clip-board. 
- If the text-input-area is blank, pressing Enter-key, the content saved in LocalStorage of your Browser will appear in the text-input-area.
- Use ";" not "," to seperate. So that "," can be used in titles. File name should be like "Get up 0H12M5S; go to school 1H5M27S; lunch 6H20M50S.mp4" to generates buttons like "Get up 0H12M5S" , "go to school 1H5M27S" , "lunch 6H20M50S".
## From 038 on : 
- When time-bar is not visable, each mouse-wheel-step video-time goes back/forward 2 seconds; 
- when mouse is near the screen-bottom each mouse-wheel-step video-time goes back/forward 10 seconds; 
- when mouse is near the screen-top each mouse-wheel-step video-time goes back/forward 1 minutes.
## From 039 on:
- Fits both time format like 1H23M6, 0H58M0S, 0H0M52S and simple time-format like 2M3, 0M23, 5M0. So as to allow more time-titles in file-name
- Press enter-key in the text-input-location, new time buttons will be generated, although you should rename the video-file to keep the new buttons.
## From 041 on:
- Use 2-row-text-area to replace the original 1-row-input-dom. More convenient in displaying and editing long file-name.
## From 043 on, click the mouse wheel in the text:
- Sort the titles by time. 
- Simplify time format, removing "S" at the end, remove "0H" if the time is smaller than 1 hour.
- Remove the blanks adjacent to ";".
- If the text is longer than 230 (max length of file-name), split the text into 230 and the longer part. The buttons are based on the whole text.
## from 045 on, when paused the mouse-wheel controls time at higher precision:
- When the mouse is in most areas and time-bar is hidden, mouse-wheel controls time at 0.5 second step.
- When mouse is near the bottom and the time-bar comes out, mouse-wheel controls time at 0.1 second step.
- When mouse is near the top and the time-bar comes out, mouse-wheel controls time at 0.01 second step.
## from 046 on, introduced play-again:
- When the video is paused at the end, click with right-mouse-key to jump to the beginning and play.
- Also simplified play/pause switch by testing cgVideo.paused.
## from 047 on: 
- The video does not pause at the end, it loops to play again and again. 
- Click the title-time input-box not only shortens the text, but also send the text to clip-board and local-storage.
