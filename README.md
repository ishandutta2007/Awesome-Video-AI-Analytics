# Awesome-Video-AI-Analytics

# Top Video AI Analytics Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Video Understanding, Surveillance Analytics & Multimodal Reasoning*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Video AI Analytics**. These tools apply computer vision, speech recognition, and large multimodal models to extract structured intelligence from video — detecting objects, tracking movement, transcribing audio, and answering natural language queries about footage.

**Examples** include Microsoft Azure Video Indexer, AWS Rekognition Video, Google Cloud Video Intelligence, Twelve Labs, Clarifai, AnyVision, BriefCam, IronYun, Valossa, and ViSenze (the category leaders).

**Open-source emphasis**: Video AI analytics is a rapidly growing open-source domain. **VideoCignium** provides a complete forensic surveillance workstation with 99.59% motion detection recall , **VideoChain** enables edge-optimized multimodal RAG for video understanding , and **Vidi2** from ByteDance delivers state-of-the-art spatio-temporal grounding . This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Microsoft Azure Video Indexer](https://azure.microsoft.com/en-us/products/ai-services/video-indexer)**  
  Cloud service for extracting insights from video and audio. Detects faces, objects, emotions, keywords, and provides transcription, translation, and content moderation. Integrated with Azure Media Services.

- **[AWS Rekognition Video](https://aws.amazon.com/rekognition/video/)**  
  AWS's video analysis service for object, face, and activity detection. Supports streaming and stored video analysis with integration into AWS Lambda and Kinesis.

- **[Google Cloud Video Intelligence](https://cloud.google.com/video-intelligence)**  
  Google's API for video analysis including label detection, shot change detection, explicit content detection, and speech transcription.

- **[Twelve Labs](https://twelvelabs.io/)**  
  Foundation model for video understanding enabling natural language search, summarization, and question answering over video content.

- **[Clarifai](https://www.clarifai.com/)**  
  AI platform with video analysis capabilities for content moderation, visual search, and custom model training.

- **[AnyVision](https://www.anyvision.co/)**  
  AI-powered video surveillance and recognition platform focused on security and access control.

- **[BriefCam](https://www.briefcam.com/)**  
  Video content analytics platform enabling rapid review of surveillance footage through object detection, tracking, and filtering.

- **[IronYun](https://www.ironyun.com/)**  
  AI video analytics platform for surveillance, offering object detection, face recognition, and behavior analysis.

- **[Valossa](https://www.valossa.com/)**  
  Video AI platform for content recognition, compliance, and media monitoring.

- **[ViSenze](https://www.visenze.com/)**  
  Visual search and image recognition platform with video commerce applications.

## Open-Source GitHub Projects

- **[VideoCignium](https://github.com/Nateram/VideoCignium)**  
  **Desktop application for automated forensic analysis of surveillance videos**, published in *SoftwareX* (2026) . Electron-based UI with Python backend. **99.59% recall, 94.23% precision, F1-score 96.83%** in motion detection; 72.35% accuracy in object classification . Processes 12-hour video blocks in ~15 minutes — **40-50x faster than manual review** . Features interactive ROI tool to filter environmental noise, YOLO-based object classification, OCR timestamp extraction, structured Excel reporting, and **fully offline operation** with SQLite storage . **The most complete open-source forensic surveillance tool** — designed for criminology departments and resource-constrained police departments .

- **[VideoChain](https://github.com/rahulsiiitm/videochain)**  
  **Edge-optimized multimodal RAG framework for video understanding**, designed for consumer GPUs (tested on RTX 3050 with 4 GB VRAM) . Late-fusion architecture combining **MobileNetV3 vision classification**, **Whisper audio transcription**, and **LLM reasoning** (Ollama/Llama 3 or Gemini) . Features adaptive keyframe extraction via Gaussian-blurred frame differencing, timestamp-synchronized multimodal alignment, and structured JSON knowledge base output . **No cloud inference dependency** for core pipeline. Best for security, retail analytics, education, and personal content search .

- **[Vidi2](https://github.com/bytedance/vidi)**  
  **ByteDance's large multimodal model for video understanding and creation**, presented in the Vidi tech report . **State-of-the-art in Spatio-Temporal Grounding and temporal retrieval**. Features temporal retrieval (find precise time ranges matching text queries), spatio-temporal grounding (draw bounding boxes around queried objects throughout video), open-ended video QA, and automatic highlight generation with titles . Available in 7B and 9B variants. **The most capable open-source video understanding model** for natural language querying of footage.

- **[reelgrep](https://github.com/pypi/reelgrep)**  
  **Local video library search and analysis tool** with a web UI . Features FTS5 full-text search across transcripts, person search with face embeddings (supports positive and negative reference images for precision), SRT subtitle export, contact sheet generation, WebP loop creation, and sub-clip extraction with stream-copy or re-encode options . **Privacy-focused** — binds to loopback only, reads exclusively from local SQLite index . **Best for researchers, lecturers, and anyone needing to search across large video collections.**

- **[YunKan](https://github.com/martin888/yunkan)**  
  **Self-hosted AI NVR/VMS in a single Docker container** . On-device AI for person/vehicle/face/plate/pose/fall detection, **no cloud dependency, no API keys required** . Features 24/7 continuous recording with motion-event highlights, AI scene understanding with natural language summaries, semantic event search, sub-second WebRTC live viewing, and Home Assistant MQTT integration . Works with any RTSP/ONVIF camera . **The most complete open-source self-hosted AI surveillance platform** — a privacy-first alternative to Frigate and ZoneMinder.

- **[FLIQ](https://pypi.org/project/fliqx/)**  
  **Lightweight face recognition acceleration layer for Python** . Single package combining detection, embedding, tracking, caching, vector search, and streaming helpers. **Runs with only NumPy installed** — optional extras unlock FastAPI, OpenCV, FAISS, and ONNX acceleration . Features face registration/recognition for still images and video streams, tracking-aware recognition, motion detection with adaptive frame scheduling, and FAISS-backed similarity search with NumPy fallback . **Best for building custom face recognition pipelines** without heavyweight dependencies.

- **[ViTCam](https://github.com/scwsoft/vitcam)**  
  **AI-powered NVR for Raspberry Pi 4/5** . Runs on CPU inference mode suitable for single-camera or lightweight monitoring . Features RTSP stream support, **RF-DETR object detection**, object tracking, detection event logging, snapshot capture, and WebRTC streaming . **Mix modes across cameras** — run AI detection on entrance cameras while keeping indoor cameras in standard NVR mode . **The most accessible entry point for DIY AI surveillance** on low-cost hardware.

- **[FluxState Edge SDK](https://pypi.org/project/fluxstate-security/)**  
  **Privacy-preserving contextual edge video analytics for enterprise security** . Features **Agentic VLM Reasoner** running Qwen2.5-VL locally via MLX on Apple Silicon, **Adaptive Intelligence** with feedback API to suppress false positives on-device, **Semantic Retrieval (RAG)** with on-device ContextLedger, and **Episodic Memory** buffering 10 minutes of scene states . **Privacy-by-design** — actively zeroes image buffers post-inference via C-level memset . Behavioral anomalies serialized to local SQLite for temporal forensics . **Best for enterprise security teams** wanting deep contextual understanding without cloud dependency.

- **[EvilEye](https://pypi.org/project/evileye/)**  
  **Extensible video surveillance analytics pipeline** with YOLO detector integration, multi-camera tracking, and zone-based analytics . Features scheduled restarts, RTSP/video file/device source support, source splitting for multi-region analysis, and configurable ROI . **Best for developers building custom surveillance pipelines** with modular detector and tracker configuration.

- **[VISION](https://github.com/Lalit-Dumka/VISION)**  
  **Comprehensive surveillance and monitoring system** combining YOLOv8 object detection, DeepFace face recognition, and PostgreSQL database management . Features face database management with embedding storage, real-time recognition with similarity scoring, zone-based movement tracking with polygon drawing, movement analytics between zones, and historical data logging with CSV export . **Best for organizations needing an integrated face recognition + zone tracking solution** with database persistence.

### Additional Strong Open-Source Options

- **YOLO26 (Ultralytics)** — Edge-focused detector released January 2026, AGPL-3.0 licensed. NMS-free inference, open-vocabulary detection via YOLOE-26x, 40.9 mAP50-95 at nano scale . **The state-of-the-art object detector for video pipelines** — note AGPL requires source disclosure for closed-source products .
- **VideoSearch-R1** — Iterative video retrieval and reasoning via soft query refinement, presented at ECCV 2026 . 2B parameter model trained for DiDeMo and ActivityNet video retrieval tasks.
- **QUAG** — Query-centric Audio-Visual Cognition Network for moment retrieval, segmentation, and step-captioning . State-of-the-art on HIREST dataset with joint multi-task learning.
- **VideoSearcher** — Multi-tool agentic reasoning for video deep research via reinforcement learning, EMNLP 2026 .
- **Lecture Mind** — Event-aware lecture summarizer using DINOv2 visual encoder and Whisper audio transcription for context-aware summaries and multimodal retrieval .

**Frameworks for building custom video AI solutions**: Combine **VideoCignium** for forensic-grade surveillance analysis with offline operation , **VideoChain** for edge-optimized multimodal RAG on consumer GPUs , and **Vidi2** for state-of-the-art natural language video querying . Use **YunKan** for a complete self-hosted AI NVR/VMS deployment , **FLIQ** for lightweight face recognition pipelines , or **ViTCam** for Raspberry Pi-based surveillance . For enterprise security with VLM reasoning, **FluxState Edge SDK** provides privacy-preserving contextual analytics . Note that true commercial platforms with managed infrastructure, pre-trained industry-specific models, and global content delivery remain primarily commercial territory; open-source stacks provide strong detection, tracking, and multimodal reasoning foundations that require integration for complete video intelligence.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Video analytics tools process sensitive footage and potentially identifiable information. Self-hosted solutions require proper security hardening, access controls, and compliance with privacy regulations (GDPR, CCPA). **Facial recognition and person tracking carry significant legal and ethical obligations** — verify local regulations before deployment.
- **YOLO26 is AGPL-3.0 licensed** — closed-source products using it must purchase an Enterprise licence or disclose source code .
- Open-source video analytics tools vary significantly in maturity. VideoCignium is designed for sequential processing and may not scale linearly for massive multi-camera city-wide deployments without optimization . Evaluate performance requirements before production deployment.
- The open-source ecosystem provides strong detection, tracking, and multimodal reasoning foundations, but managed infrastructure, industry-specific pre-trained models, and enterprise support remain primarily commercial offerings.

---

**Made for security engineers, forensic analysts, video AI researchers, and developers building video intelligence systems.**  
Let's make video AI analytics more open, transparent, and privacy-respecting.
