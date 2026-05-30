# MediaConverter
Watermark Removal, Video Conversion, Compression, Trimming
[中文](./README_zh.md)

> **Browser-based AI Media Post-Processing Tool — Watermark Removal · Video Conversion · Compression · Trimming**
> ⚠️ Currently in Beta — feedback and bug reports are welcome

## Overview

MediaConverter is a fully browser-based media processing tool that requires no installation and no server uploads.  
It is primarily designed to remove watermarks from AI-generated content (e.g., images from nano banana, videos from Gemini Omni Flash) and includes a set of practical video processing utilities.

## Features

### 1. Watermark Removal

Remove watermarks embedded in the lower-right corner of AI-generated content:

- Supports watermark removal from **nano banana**-generated images
- Supports watermark removal from **Gemini Omni Flash**-generated videos
- Fully customizable overlay **position** and **size** to precisely align with the original watermark
- 💡 **Tip:** When processing videos, setting `Alpha Scale` to `0.6` is recommended for optimal results

### 2. Video Conversion

- Converts most common video formats to **MP4**

### 3. Video Compression

- Reduces file size by adjusting **bitrate** and **resolution**

### 4. Video Trimming

- Set custom start and end timestamps to extract and keep only the desired portion of a video

## Tech Stack

| Component | Description |
|-----------|-------------|
| [mediabunny](https://github.com/Vanilagy/mediabunny) | Primary video processing engine for common formats |
| [ffmpeg.wasm](https://github.com/ffmpegwasm/ffmpeg.wasm) | Fallback engine for formats not supported by mediabunny |

Special thanks to **[Allen Kuo](https://github.com/allenk/GeminiWatermarkTool)** for the original concept and inspiration behind the watermark removal feature.

## Known Limitations

- Some watermarks on videos or images may not be fully removed (ongoing improvement)

## Disclaimer

> This tool is intended for personal and lawful use only.  
> **Do not use this software for any infringing or illegal purposes.**  
> Under no circumstances shall the author be held liable for any claims, damages, or other liabilities arising from the use of this software.
