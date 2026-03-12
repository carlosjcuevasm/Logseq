- Chatgpt roadmap I found great
  collapsed:: true
	- **Summary:**
	- For a **Senior Video Engineer (WebRTC + livestream platform)** role like Eureka Labs, interviews almost always revolve around **system design, media pipelines, WebRTC fundamentals, and debugging streaming issues**.
	- Below are **10 very common questions** for roles using **WebRTC, Mediasoup, FFmpeg, RTMP, and HLS**, plus the **kind of reasoning a senior engineer is expected to demonstrate**.
	- ---
	- # 10 Questions You’re Very Likely to Get
	- ---
	- # 1. “How would you design a livestreaming platform?”
	- They want to see **architecture thinking**.
	- A solid high-level answer:
	- ```
	  camera capture
	  ↓
	  WebRTC ingest
	  ↓
	  SFU routing (Mediasoup)
	  ↓
	  optional recording / transcoding
	  ↓
	  RTMP output
	  ↓
	  HLS packaging
	  ↓
	  CDN delivery
	  ↓
	  players
	  ```
	- Key things to mention:
		- **WebRTC for real-time viewers**
		- **HLS for scale**
		- **Mediasoup SFU for routing**
		- **FFmpeg for processing / recording**
		- **CDN for global distribution**
	- This architecture is similar to systems used by platforms like Twitch and YouTube Live.
	- ---
	- # 2. “What problem does an SFU solve?”
	- An **SFU (Selective Forwarding Unit)** routes streams between participants.
	- Instead of mixing streams, it forwards them.
	- ```
	  publisher
	  ↓
	  SFU
	  ↓
	  many viewers
	  ```
	- Advantages:
		- lower CPU usage
		- lower latency
		- scalable
	- Contrast with **MCU (Multipoint Control Unit)**:
	- MCU mixes streams into one output → expensive and higher latency.
	- Modern platforms almost always use **SFU architectures**.
	- ---
	- # 3. “What is simulcast and why is it important?”
	- Simulcast means the sender publishes **multiple quality versions simultaneously**.
	- Example:
	- ```
	  1080p stream
	  720p stream
	  360p stream
	  ```
	- The SFU chooses which stream each viewer receives.
	- Benefits:
		- adaptive bitrate
		- efficient bandwidth usage
		- scalable delivery
	- This is widely used in WebRTC platforms like Zoom Video Communications.
	- ---
	- # 4. “How does WebRTC establish connections?”
	- Core process:
	- ```
	  1. signaling
	  2. ICE negotiation
	  3. STUN/TURN discovery
	  4. RTP media transport
	  ```
	- Key technologies:
		- SDP (session description)
		- ICE (candidate negotiation)
		- STUN (public IP discovery)
		- TURN (relay when direct connection fails)
	- If they ask about NAT traversal → this is the answer.
	- ---
	- # 5. “How do you reduce livestream latency?”
	- Typical approaches:
	- Reduce segment size
	- Example:
	- ```
	  10s segments → high latency
	  2s segments → lower latency
	  ```
	- Other strategies:
		- WebRTC transport
		- LL-HLS
		- optimized buffering
		- faster encoding pipelines
	- But tradeoff:
	- ```
	  lower latency
	  ↓
	  more instability risk
	  ```
	- Senior engineers **always mention the tradeoff**.
	- ---
	- # 6. “How do you scale a livestreaming platform?”
	- Typical architecture:
	- ```
	  multiple SFU nodes
	  ↓
	  load balancer
	  ↓
	  regional clusters
	  ↓
	  CDN delivery
	  ```
	- Scaling methods:
		- horizontal scaling
		- geographic distribution
		- simulcast
		- viewer edge delivery
	- Large platforms also use **multi-region infrastructure**.
	- ---
	- # 7. “How does FFmpeg fit into livestreaming platforms?”
	- FFmpeg is usually used for:
		- transcoding
		- recording
		- restreaming
		- packaging
	- Example pipeline:
	- ```
	  WebRTC ingest
	  ↓
	  FFmpeg
	  ↓
	  RTMP output
	  ↓
	  HLS packaging
	  ```
	- Common uses:
		- VOD recording
		- stream clipping
		- adaptive bitrate ladder generation
	- ---
	- # 8. “How would you troubleshoot buffering or playback issues?”
	- A senior answer traces **the pipeline**.
	- Possible causes:
	- ```
	  encoder bitrate too high
	  ↓
	  segment sizes too large
	  ↓
	  CDN cache miss
	  ↓
	  player buffer underrun
	  ```
	- Steps to debug:
		- inspect encoder output
		- check segment duration
		- analyze CDN logs
		- analyze player telemetry
	- Streaming debugging is **pipeline debugging**.
	- ---
	- # 9. “How do you measure video quality?”
	- Typical metrics:
		- bitrate
		- frame drops
		- startup time
		- buffering ratio
	- Advanced metrics include:
		- **VMAF** (video quality metric)
		- QoE scoring
	- Netflix uses VMAF heavily for encoding optimization.
	- ---
	- # 10. “What tradeoffs exist in streaming system design?”
	- A strong answer highlights tradeoffs:
	- Latency vs stability
	- ```
	  smaller segments
	  ↓
	  lower latency
	  ↓
	  higher CDN overhead
	  ```
	- Quality vs bandwidth
	- ```
	  higher bitrate
	  ↓
	  better video
	  ↓
	  higher delivery cost
	  ```
	- Scalability vs complexity
	- ```
	  WebRTC scale challenges
	  ↓
	  HLS scale advantages
	  ```
	- Senior engineers constantly reason about **tradeoffs**.
	- ---
	- # Things You Should Be Comfortable Explaining
	- Before the interview, make sure you understand:
	- ### WebRTC basics
		- ICE
		- STUN
		- TURN
		- RTP
		- SDP
	- ### Streaming protocols
		- RTMP
		- HLS
		- WebRTC
		- SRT
	- ### Media pipeline
	- ```
	  capture
	  encode
	  package
	  deliver
	  playback
	  ```
	- ### Media servers
		- Mediasoup
		- SFU architecture
	- ---
	- # One Last Interview Tip
	- When answering questions, **explain pipelines**, not tools.
	- Instead of saying:
	- > “I know FFmpeg and WebRTC.”
	- Say something like:
	- > “In a typical livestream pipeline, WebRTC handles low-latency ingest while FFmpeg can be used for recording, transcoding, or restreaming into HLS distribution.”
	- That framing signals **systems engineering thinking**, which is exactly what they want in a **Senior Video Engineer**.
	- ---
	- If you want, I can also show you **3 architecture diagrams that appear extremely often in livestreaming platforms** (including Mediasoup setups). Understanding those will make half the interview questions trivial.