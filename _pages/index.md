---
layout: home
permalink: /
title: "Coming soon:"
---

## Unleash Your Voice | The Ultimate Open-Source Vocoder

Welcome to the next generation of vocoding!
I’m developing a fully open-source vocoder designed for musicians, synth lovers, and DIY audio enthusiasts. 
While it's development is currently in progress, you can follow the creation step by step through blog updates and videos as I fine-tune every detail.

This vocoder will be fft based meaning you can experience high-quality vocoding without traditional bandpass filter limitations.

<div align="center">

<h2>Teaser</h2>

</div>
<div style="position: relative; display: inline-block; max-width: 100%;">

    <video id="promoVideo" src="/assets/images/Promo.mp4" loop muted playsinline style="max-width: 100%; height: auto; border-radius: 8px; display: block;"></video>

    <button id="playButton" style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); background: rgba(0,0,0,0.6); border: none; border-radius: 50%; width: 64px; height: 64px; cursor: pointer; display: flex; align-items: center; justify-content: center;">
        <svg width="32" height="32" viewBox="0 0 32 32" fill="#fff" xmlns="http://www.w3.org/2000/svg">
            <polygon points="10,8 26,16 10,24"/>
        </svg>
    </button>

</div>

<script>
    const video = document.getElementById('promoVideo');
    const playButton = document.getElementById('playButton');

    playButton.addEventListener('click', function() {
        video.play();
        playButton.style.display = 'none';
        video.muted = false;
    });

    // Add click to pause after video plays
    video.addEventListener('click', function() {
        if (!video.paused) {
            video.pause();
            playButton.style.display = '';
        }
    });
    video.addEventListener('play', function() {
        playButton.style.display = 'none';
    });
</script>

## How can you get one?
Once the vocoder is a finished product, you’ll have options! 
It will be available as:
- A fully assembled unit – Plug and play for the people that just want to make music (Option 1).
- DIY kit - Build it yourself with all the necessary parts ready to go (Option 2).
- Build your own - Get all the files from the github page and assemble the vocoder from scratch (Option 3).

Follow my journey! Blog posts and videos will document every step of development.

### Want to be among the first to get your hands on it? Sign up now to show your interest and stay updated!✨✨
{: .notice--success}

<form
    action="https://formspree.io/f/mqaplove"
    method="POST"
>
    <label>
        Your email📨
        <input type="email" name="email">
    </label>
    <label>
        add a message, ideas and feedback are always welcome🙂
        <textarea name="message"></textarea>
    </label>
    <fieldset>
        <legend>What version would you be interested in?:</legend>
        <label>
            <input type="radio" name="option" value="option 1 (Full)"> Option 1 (Fully sssembled)
        </label>
        <label>
            <input type="radio" name="option" value="option 2 (DIY)"> Option 2 (DIY)
        </label>
        <label>
            <input type="radio" name="option" value="option 3 (FREE)"> Option 3 (Build your own)
        </label>
    </fieldset>
    <button type="submit">Send</button>
</form>
