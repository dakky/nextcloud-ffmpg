
<div align="center">
	<img src="https://raw.githubusercontent.com/nextcloud/server/master/apps/theming/img/nextcloud.svg" alt="Nextcloud Logo" width="120"/>
	<h1>nextcloud-ffmpeg</h1>
<p align="center">
	<a href="https://github.com/dakky/nextcloud-ffmpeg/actions">
		<img src="https://github.com/dakky/nextcloud-ffmpeg/actions/workflows/build.yml/badge.svg" alt="Build Status" />
  </a>
</p>
	<p><strong>Nextcloud Docker image with integrated FFmpeg for advanced media processing</strong></p>
	<br/>
</div>


## 🚀 Overview

This project provides a custom Docker image for [Nextcloud](https://nextcloud.com/) with [FFmpeg](https://ffmpeg.org/) pre-installed. FFmpeg enables advanced media processing, such as video previews, transcoding, and audio extraction, directly within your Nextcloud instance.

## ✨ Features

- **Nextcloud + Apache**: Based on the official Nextcloud Apache image
- **FFmpeg Integration**: Enables video previews, transcoding, and more
- **Easy Deployment**: Ready-to-use Docker setup
- **Minimal Footprint**: Installs only required packages

## 🐳 Quick Start

```sh
git clone https://github.com/dakky/nextcloud-ffmpg.git

# Clone the repository (if needed)
git clone https://github.com/dakky/nextcloud-ffmpeg.git
cd nextcloud-ffmpeg


# Build the Docker image
sudo docker build -t nextcloud-ffmpeg .

# Run the container
sudo docker run -d \
	-p 8080:80 \
	-v nextcloud_data:/var/www/html \
	--name nextcloud-ffmpeg \
	nextcloud-ffmpeg
```

Access your Nextcloud instance at [http://localhost:8080](http://localhost:8080).


## ⚙️ Requirements & Architecture

- Docker (v20+ recommended)
- ~2GB RAM for smooth media processing
- **Only the amd64 architecture is supported and built by this image.**

## 🛠️ Customization

You can extend this image by adding more packages or custom scripts in the Dockerfile.

## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## 🤝 Contributing & Support

Pull requests and issues are welcome! For questions, open an issue or contact the maintainer:
- **GitHub**: [dakky](https://github.com/dakky)

---

<div align="center">
	<sub>Made with ❤️ for Nextcloud & FFmpeg</sub>
</div>
