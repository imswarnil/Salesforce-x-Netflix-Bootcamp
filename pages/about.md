---
layout: page
menu: false
date: '2020-02-27 01:53:59'
title: About
description: Some description.
permalink: /about/
---
<style>

    .video-container {
      position: relative;
      overflow: hidden;
      width: 100%;
      max-width: 800px;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      margin: 0 auto;
      cursor: pointer;
    }

    .video-overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      background: rgba(0, 0, 0, 0.5);
      opacity: 0;
      transition: opacity 0.3s ease;
    }

    .video-overlay:hover {
      opacity: 1;
    }

    .play-icon {
      color: #fff;
      font-size: 4em;
      cursor: pointer;
    }

    video {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  </style>
<div class="video-container">
  <div class="video-overlay" onclick="playPause()">
    <i class="play-icon">&#9658;</i>
  </div>
  <video id="myVideo" controls preload="metadata">
    <source src="/videos/1. Introduction.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

<script>
  var video = document.getElementById("myVideo");

  function playPause() {
    if (video.paused) {
      video.play();
    } else {
      video.pause();
    }
  }
</script>

# About

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
