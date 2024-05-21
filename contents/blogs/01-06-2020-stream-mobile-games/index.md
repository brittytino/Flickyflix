---
slug: /blog/instagram-live-stream-pubg-call-of-duty-phone-OBS-Studio
layout: blog
published: true
date: 2020-06-01
title: Stream PUBG or Call Of Duty mobile games to Instagram Live with OBS Studio and Streamon
description: Learn how to stream your mobile gaming sessions of PUBG, Call of duty from Android device to Instagram Live using OBS Studio and Streamon easily.
author: Musthaq Ahamad
username: haxzie
youtube: https://www.youtube.com/watch?v=TyyuMCTpjNY
keywords:
  - instagram
  - OBS studio
  - PUBG mobile
  - Call of duty mobile
  - instagram live
  - streaming
cover_image: ./gameplay.png
---

There has been a huge rise in gaming with smart phones these days. If you game on your smartphones, ever wondered how to stream your live gameplay to your friends? In this article we'll learn how to stream mobile games like PUBG mobile, Call Of Duty Mobile or any game on your smartphone to Instagram Live.

Follow the below steps to start streaming almost anything on your mobile screen to Instagram live with [Streamon](https://getstreamon.com). Before we start, make sure you have the following setup and softwares installed on your system.

- An Andoid phone with your favourite mobile game (Unfortunately, Iphones won't be able to work in this method)
- An Instagram account (Obviously)
- [Screen Stream Over HTTP](https://play.google.com/store/apps/details?id=info.dvkr.screenstream&hl=en) app on your android phone
- A Windows/Linux desktop or laptop with [OBS Studio](https://obsproject.com/) installed
- Install [Streamon](https://getstreamon.com) on your desktop or laptop

## 1. Streaming your android device to your PC

<Image src="./screen-stream.png" alt="Screen Stream app"/>
<span style="text-align: center; display: block; font-size: 1rem">Screen Stream Over HTTP app on Play store</span>

Install and Open the [Screen Stream Over HTTP](https://play.google.com/store/apps/details?id=info.dvkr.screenstream&hl=en) app on your android phone and click on the **play** button on the bottom to start streaming your screen over HTTP. Make sure both your laptop/desktop and phone is on the same wifi network. Note down the URL shown in the app and open it in the browser.

<Image src="./screen-stream-home.png" alt="Screen Stream app"/>
<span style="text-align: center; display: block; font-size: 1rem">Screen Stream app's home page</span>

Once the stream is started, open a new browser window in your PC and go to the **device address** provided on the app's screen.

<Image src="./device-on-browser.png" alt="device screen on browser"/>
<span style="text-align: center; display: block; font-size: 1rem">Your device screen on browser</span>


## 2. Setting up OBS Studio

Head over to OBS Studio's [home page](https://obsproject.com/) to download and install the Software on your system. Once the installation is complete open OBS Studio.

<Image src="./obs-ss.png" alt="OBS Studio Start Screen"/>
<span style="text-align: center; display: block; font-size: 1rem">OBS studio start screen</span>

### Configuring a new stream profile and video output

Most of your viewers will be on a mobile device and mobile device screens are of a different aspect ration than your computer. Click on **Profile** menu on OBS at the top and click on **New Profile** and name the Profile as `Instagram Streaming`.

Now, Click on **settings** in the bottom right panel and go to the **Video tab**. Change the **Base (canvas) Resolution** to any of the **9:16** aspect ratio, in my case it's `900x1600` of my monitor. And, set the **Output (scaled) resolution** to `720x1280`. Click on **Apply** and **OK**.

<Image src="./obs-video-settings.png" alt="OBS video settings"/>
<span style="text-align: center; display: block; font-size: 1rem">OBS video settings screen</span>

### Adding your phone screen as video source

Once we configured the video output, we need to add a video source. Click on the **+** icon from the bottom left, second panel which says **Sources** and click on `Window Capture` and choose the **Screen Stream** browser window on **Window** selcetion which is streaming your mobile screen. Once, the device is being added you can simply use the handles on the preview to adjust the view to the canvas. If you want to rotate the view, right click on the preview, select transform and choose **Rotate 90 degrees**.

<Image src="./scrcpy-obs.png" alt="Device screen on OBS"/>
<span style="text-align: center; display: block; font-size: 1rem">Your Device Screen On OBS</span>

You can now open your favourite game on your phone and make sure you have rotated the preview screen as I mentioned above to 90 degrees.

<Image src="./game-screen-on-obs.png" alt="Device screen on OBS"/>
<span style="text-align: center; display: block; font-size: 1rem">Your Device Screen On OBS</span>

> Currently there is no official way to capture your phone's audio into OBS, we will update this article soon if we find any reliable method. For now, you can use your computer's connected mic to listen to your phone's audio

## 3. Starting an Instagram Live Stream with Streamon

Once you haver configured your streaming setup, you can now use [Streamon](https://getstreamon.com) to start an Instagram Live session. Open **Streamon (instagram-live-streamer)** on your PC and login to your Instagram account. After logging in click on **Start live stream**, you will be greeted with a screen containing your **Stream URL** and **Stream key**. DONOT click on **GO LIVE** yet!

<Image src="./streamon-creds.png" alt="Streamon - Instagram live credentials"/>
<span style="text-align: center; display: block; font-size: 1rem">Streamon - Instagram live credentials</span>

### Configuring OBS Studio with stream credentials

Now, open your OBS studio instance and click on settings and go to **Stream** tab. In the service, make sure to select **Custom** and then copy paste the **Server URL/Stream URL** and the **Stream Key** from the Streamon app into OBS. Make sure the `use authentication` check box is **Unchecked**. Click on apply and ok.

<Image src="./obs-stream-config.png" alt="Streamon - Instagram live"/>
<span style="text-align: center; display: block; font-size: 1rem">Configuring OBS Stream configuration</span>

Now, on the bottom right panel near the **Settings Button** click on **Start Stream!**. Once the stream is started, quickly go to the Streamon app and click on **Go Live** Button. Voila! You are now live on Instagram streaming through OBS Studio. You can click on the comment icon on the bottom to see your live comments from Instagram.

<Image src="./streamon-live.png" alt="Streamon - Instagram live"/>
<span style="text-align: center; display: block; font-size: 1rem">Streamon - Instagram live</span>

If you wish to see your stream and live chat on Instagram, simply sign in to your Instagram account from your PC's Browser and goto `https://instagram.com/USERNAME/live`. Replace the `USERNAME` with your Instagram username.

<Image src="./live-stream.jpeg" alt="Streamon - Instagram live"/>
<span style="text-align: center; display: block; font-size: 1rem">Live stream on Instagram</span>




> Please Note, you won't be able to view your live stream from the Instagram mobile app or desktop directly. You can see the stream through the above method or login via a different Instagram account to view your stream.

To Stop the live stream, simply click on stop live stream from your OBS Studio and then from the Streamon app.

### Stuck with something? Need help?
Head over to our community channel on [Telegram (t.me/streamonhq)](https://t.me/streamonhq) or Tweet to us at [@streamonhq](https://twitter.com/streamonhq) to get help from the community.

Found this project helpful? Consider supporting us via [BuyMeACoffee](https://buymeacoff.ee/haxzie) 💖 