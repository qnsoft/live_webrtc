# webrtc 插件

提供通过网页发布视频到live_sdk，以及从live_sdk拉流通过webrtc进行播放的功能

# 基本原理

通过浏览器和live_sdk交换sdp信息，然后读取rtp包或者发送rtp的方式进行

# API
- /api/webrtc/play?streamPath=live/rtc
用于播放live/rtc的流，需要在请求的body中放入sdp的json数据，这个接口会返回服务端的sdp数据
- /api/webrtc/publish?streamPath=live/rtc
同上
