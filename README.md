# OS-project
This repository contains code for operating system project from Banana9Fingers group.

🎵 YouTube Mood-Based Music Video Downloader

This project is a Python-based tool that downloads music videos from YouTube based on user-defined moods (e.g., happy, sad, chill). It uses the YouTube Data API to search for videos, and yt-dlp to download them. To evaluate performance, the tool supports sequential processing, multithreading (ThreadPoolExecutor), and multiprocessing. It is optimized to run on Google Colab, using CPU, GPU, or TPU environments (although video downloading is CPU/I/O-bound).

📌 Features

🔍 Search YouTube videos by mood using the YouTube Data API
📥 Download videos or extract audio using yt-dlp
🧵 Concurrent downloads via:
Sequential Processing
ThreadPoolExecutor (Multithreading)
Multiprocessing
📊 Benchmark and analyze performance on CPU, GPU, and TPU
📄 Generate detailed reports on speed, CPU/memory usage, and I/O efficiency
