# OS-project
This repository contains code for operating system project from Banana9Fingers group.

# 🎵 YouTube Mood-Based Music Video Downloader

This project is a Python-based tool designed to download music videos from YouTube based on user-defined **moods** (e.g., happy, sad, relaxing). It integrates the **YouTube Data API** for video search and **yt-dlp** for downloading, and it compares performance across **sequential**, **multithreading (ThreadPoolExecutor)**, and **multiprocessing** methods. It is designed for experimentation on **Google Colab** using CPU, GPU, or TPU environments.

---

## 📌 Features

- 🔍 Search music videos by mood using YouTube Data API
- 🎥 Download full videos or extract only audio using `yt-dlp`
- 🧵 Use of ThreadPoolExecutor for efficient I/O-bound downloads
- 🧠 Support for multiprocessing to parallelize downloads
- 🔁 Sequential baseline for performance comparison
- 📊 Analyze speed and resource use across different processing types

---

## 🧪 Usage

In this project, you can use three different notebooks to compare the performance of **sequential processing**, **multithreading**, and **multiprocessing**.

1. **Sequential Processing**  
   Run the `OS_project_normal.ipynb` to download videos sequentially (one at a time).

2. **ThreadPool (Multithreading)**  
   Run the `OS_project_threaded.ipynb` to download videos concurrently using `ThreadPoolExecutor`.

3. **Multiprocessing**  
   Run the `OS_project_multiprocess.ipynb` to download videos using multiple processes in parallel.

Each notebook represents a different processing approach. Simply open and execute the relevant notebook in your Jupyter environment or Google Colab.

---

## 🧠 Technology Notes

- **yt-dlp** is a powerful command-line tool for downloading videos and audio from YouTube and many other platforms. It supports post-processing operations such as audio extraction, subtitle downloads, and more.
  
- **ThreadPoolExecutor** in Python is used for I/O-bound concurrency, which is especially useful when downloading many small files concurrently. This approach enhances download speeds by overlapping I/O operations and utilizing system resources efficiently.

- **Multiprocessing** is ideal for CPU-bound tasks or when thread-based downloads are rate-limited. It allows the program to run multiple processes in parallel, utilizing multiple cores of the CPU.

---

## 👨‍🏫 Academic Purpose

This project was developed to demonstrate the application of concurrent programming techniques in Python using a real-world API and tool (**yt-dlp**). It helps analyze **resource consumption** and **performance trade-offs** between:

- Sequential processing  
- Multithreaded processing using `ThreadPoolExecutor`  
- Multiprocessing with `multiprocessing` module

Experiments were conducted on **Google Colab** to evaluate hardware effects across:

- **CPU**
- **GPU**
- **TPU**

These tests focused on **I/O-bound workloads** (such as video and audio downloads), providing insights into how parallelism and different hardware configurations impact the overall system performance.


