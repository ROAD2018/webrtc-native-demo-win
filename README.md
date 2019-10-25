# update2019
As time passes, I changed my mind. I would suggest people integrate WebRTC based on the PeerConnection API, not the rtc_media API. Because rtc_media API is not stable, which means it maybe removed someday. When you upgrade WebRTC, you may have to change lots of integration code.

# webrtc-native-demo-win

WebRTC native demo on Windows without signaling, just showing how to make use of webrtc video/audio engine.

The reason is that I can only get Javascript sample code by Google: https://github.com/webrtc/samples. 
But sometimes people wants to make use of WebRTC native api to set up a video/audio real-time commucation Application.

There are two native demo in the WebRTC source code: peerconnection_client for Windows, AppRTCMobile for Android/iOS. 
But it's not simple enough to show how to use WebRTC video/audio engine API, because both demo set up based on libjingle_peerconnection API, not rtc_media.
Take peerconnection_client as example:
![webrtc-projects-dependency](/webrtc-projects-dependency.png)

## Dev Status

WebRTC M59 commit id: 61fe801ad874104a2d461083f53caee4c19c51b6

| Plan          | Status |
| - | - |
| Video capture | done   |
| video render  | done   |
| video codec   |        |
| udp transport |        |
| audio         |        |

