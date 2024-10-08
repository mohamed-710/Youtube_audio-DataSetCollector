
# 🎧 YouTube Audio & Caption Downloader




## ✨ Why This Project Was Built
This project was built to automate the process of downloading audio from YouTube and obtaining manual captions. By focusing on mixed-language captions (Arabic and English), it provides a convenient tool for researchers or developers working on multilingual data or audio-related applications.





## 🛠 Problem It Solves
Manually downloading audio and extracting captions from YouTube is time-consuming and often complex, especially for large channels or playlists. This project automates the process, allowing you to quickly:
- Fetch audio from YouTube 🎶
- Split it into chunks based on caption timings ✂️
- Save captions and metadata easily 📝




## 🚀 Features
- 📥 Download audio from individual YouTube **videos**, **channels**, or **playlists**.
- 🌐 Extract and filter captions, focusing on mixed **Arabic** and **English** content.
- ✂️ Cut the audio into segments based on caption timestamps.
- 📝 Automatically generate a **metadata** file containing audio file names and corresponding captions.




## 🖥 How to Run the Code



### 1. 📦 Prerequisites

Make sure you have the following Python libraries installed:

- Install dependencies from the `requirements.txt`:

```bash
pip install -r requirements.txt
```


### 2. 📄 Prepare the Input



- Create a text file (e.g., `urls.txt`) containing the YouTube URLs (one per line) that you want to process.

### 3. 🏃 Run the Script



Run the script using the following format:

```bash
python main.py --link_type [video|channel|playlist] --audio_type [all|mix_only] --output_dir [path_to_output] --urls_file [path_to_urls_file]
```


#### Arguments:
- `--link_type`: Specify the type of YouTube link (`video`, `channel`, or `playlist`).
- `--audio_type`: Select either `all` audio or only those with `mix_only` (Arabic and English) captions.
- `--output_dir`: Specify the output directory for audio files.
- `--urls_file`: Path to the text file containing YouTube URLs.


### 💡 Example Command

```bash
python main.py --link_type video --audio_type mix_only --output_dir ./audio --urls_file ./urls.txt
```


### 4. 📂 Output


The script will generate:
- 🎶 Audio chunks saved in the specified output directory.
- 🗒️ A `metadata.jsonl` file, containing the file name of each audio chunk and its corresponding caption.



