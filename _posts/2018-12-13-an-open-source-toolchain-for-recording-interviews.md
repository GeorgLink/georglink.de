---
id: 745
title: An Open Source Toolchain for Recording Interviews
date: 2018-12-13T16:50:28-06:00
author: Georg Link
layout: post
guid: http://www.georglink.de/?p=745
permalink: /2018/12/13/an-open-source-toolchain-for-recording-interviews--745
categories:
  - Erkenntnisgewinne
  - Forschung
  - Open Source
  - Research
tags:
  - Audacity
  - Blender
  - How To
  - Interviews
  - OBS Studio
---
**TL;DR:** _When recording through conferencing system is unavailable, I use three open source tools to record interviews: OBS Studio, Blender, and Audacity._  


As a qualitative researcher, I enjoy engaging with people directly and occasionally I want to record an interview. I conducted XL (roman numeral) interviews as part of my PhD and I figured out how to capture the audio and transcribe it. A primary concern is the quality of a recording. Because I am undoubtedly not alone, I describe here lessons learned and my open source tool chain.  


My first attempt at recording an interview involved an old-school telephone on speakerphone and my smartphone with an audio recording app. The audio quality was abysmal. My voice was clear, but my informant’s voice was distorted through the analog transformation between phone speaker and smartphone microphone. I never tried this again.  


The best solution is using the conferencing system that my university provides. The system allows my informants to connect via app, browser, or phone. In my experience, about 90% of informants join via app and activate their camera, which makes for a great conversation. The recording quality is only dependent on the microphones quality. Sometimes, I ask informants if they have an alternative they switch between a headphone to a built-in microphone.  


This optimal solution is not always practical and some informants prefer to use alternative ways to connect, such as Skype, Jitsi, Meet.me, GoToMeeting, or a conferencing system they control. When I need to make a phone call, I use Google voice from my laptop. I developed a toolchain of open source software that allows me to record an interview in such settings. I use three tools: OBS Studio, Blender, and Audacity.  


[OBS Studio](https://obsproject.com/) (Open Broadcaster Software Studio) allows to capture anything on my screen and record in-going and out-going audio. I simply record the audio output from my computer and my microphone input during an interview. The quality is the same as directly recording it through a conferencing solution. The downside is that OBS requires computing resources and at times bogs down my laptop. I end up with a *.flv video file that contains the desired audio.  


[**Blender**](https://www.blender.org/) is a 3D modeling software but has powerful video editing capabilities. I recommend [Mikeycal Meyers’ tutorial](https://www.youtube.com/playlist?list=PLjyuVPBuorqIhlqZtoIvnAVQ3x18sNev4) on how to get setup. Blender is overkill for extracting audio, but it is a tool I know. Once the \*.flv file is loaded into Blender, I export the audio, without doing any editing. I end up with a \*.flac audio file. **  
** 

Finally, I use [**Audacity**](https://www.audacityteam.org/) to cut the audio and tweak it. I edit any audio, whether recorded by OBS or a conferencing system, with three goals in mind. First, I cut the beginning and end because small talk is not important to my analysis. Second, I check to make sure my informant is audible. When the audio is too quiet, I boost it using _Effect &#8211;> Compressor…_ for the whole audio or _Effect &#8211;> Amplify…_ for small sections. Third, I shorten pauses using _Effect &#8211;> Truncate Silence…_ which saves fees on transcription services. I export the final audio as an *.mp3 audio file.  


After generating a good quality audio file, I need to transcribe the interview. I transcribed one interview myself using [OTranscribe](https://otranscribe.com/) and it took me six hours for a one hour interview because I worked to get every word and half sentence and expression right. I quickly learned that this level of detail is hindering me and a more streamlined transcript is easier to analyze. After making this experience, I value having a research grant that pays for a transcription service and I am a returning customer of [rev.com](https://www.rev.com/).