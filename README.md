# SnapFind
Find any moment in video, with one sentence.

## System Compatibility
This software is **only available for Windows**. For Mac or Linux users, please use the Python version:  
https://github.com/XinzhengDu/SnapFind_Python  

## Open Source & Technical Basis
The source code before compilation is available at:  
https://github.com/XinzhengDu/SnapFind_Python  

## 100% Local Execution (Privacy Compliance)
Core Logic: All video parsing, model inference, and content retrieval are processed **entirely on the user's device**.  
No user data (videos, images, text) is uploaded to any server. This complies with global privacy regulations:  
- China: Personal Information Protection Law (PIPL)  
- EU: General Data Protection Regulation (GDPR)  
- US: California Consumer Privacy Act (CCPA)  

## Important Note
Currently, **English query terms are better supported** than other languages. If search results are inaccurate, translate your query into English before input.

## Prerequisites
Before use, you must download the following model and tokenizer files:  
- siglip_vision.onnx  
- siglip_text.onnx  
- tokenizer.json  

Download link: https://www.modelscope.cn/models/XinzhengDu/siglip2-base-patch16-224-onnx/files  
Place all files in the `model` folder.

## Beta Features (Currently Available)
1. Content matching: Match search terms with videos, images, and documents. Queries support descriptions of time, location, people, and scenarios.  
2. OCR matching: Recognize and match text in videos/images (requires more computing power).  
3. Feature caching: Cache file features to reduce waiting time for subsequent calls.  
4. Search results: View thumbnails and open source files directly from the results page.  
5. Frame interval customization: Set N-second frame capture intervals for long/short videos to extract features.  
6. Precision adjustment: Optimize cache precision for different scenarios to maximize computing resource utilization (Settings > File).  
7. Low-spec device support: Set longer frame intervals for devices with limited computing power (Settings > File).  
8. Top-N results: Return the N most relevant results (more results = longer wait time; reduce N for time-sensitive use cases).

## Upcoming Features (In Development)
- GPU acceleration: 90% complete (supports video loading and model inference via GPU).  
- Image upload for search: 90% complete (search for relevant content by uploading images).  
- Video player integration: Jump to specific timestamps, add screenshot/GIF features (for meme creation), and audio positioning (for video segmenting).  
- Direct file navigation: Open files at specific timestamps (requires designated video player installation).  
- Idle-time feature computation: Automatically compute file features when the computer is idle (pauses if resource-intensive programs run).  
- Real-time monitoring analysis: Analyze risk levels of live surveillance content (e.g., monitor pet status).  
- Vertical model training: Train domain-specific models (requires significant computing power and datasets).

## Use Cases
- Locate video timestamps by human actions (e.g., "find the 10th minute where someone waves hands").  
- Fast navigation in tutorial videos: Jump directly to relevant sections without watching the entire video.  
- Class video indexing: Quickly find key moments in recorded lectures.  
- Surveillance footage analysis: Avoid manual frame-by-frame checking (e.g., "find the moment a package is delivered").  
- Image-based search: Upload a photo (e.g., a group photo) to find related historical images/videos.

## User Agreement & Disclaimer
1. **Legitimate Use Only**: This software is strictly for legal and compliant use cases. It is prohibited for illegal surveillance, invasion of privacy, or other unlawful activities.  
2. **User Liability**: Users assume full responsibility for all consequences of using this software. The developer shall not be liable for any misuse.  
3. **Content Restrictions**: The software restricts retrieval of illegal content (e.g., pornography, violence) to comply with applicable laws and regulations.  
