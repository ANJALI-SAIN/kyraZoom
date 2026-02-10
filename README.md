kyraZoom is a real-time video conferencing application built using WebRTC, designed to demonstrate peer-to-peer communication, signaling flow, and scalable frontend architecture for live interactions.
This project focuses on how video calls actually work under the hood, not just UI.

# Features

*Real-time video & audio calling
*Peer-to-peer communication using WebRTC
*Unique room-based connections
*Media device access (camera & mic)
*Dynamic join/leave handling
*Responsive UI for desktop & mobile
*Graceful error handling for media permissions

#Tech Stack

Frontend:

*JavaScript (ES6+)
*HTML5, CSS3
*WebRTC APIs
*RTCPeerConnection
*getUserMedia
*RTCSessionDescription
*Signaling (Basic)
*Socket.io / WebSocket (for SDP & ICE exchange)

#Tools

*Git & GitHub
*VS Code

Browser DevTools:

*System Design (High Level)
User A (Browser)              User B (Browser)
   |                                |
   |---- Offer (SDP) -------------->|
   |<--- Answer (SDP) --------------|
   |---- ICE Candidates ----------->|
   |<--- ICE Candidates ------------|
   |                                |
   |====== Peer-to-Peer Media ======|


* Media streams flow directly between peers,
* Signaling server is used only to exchange connection metadata.

# WebRTC Call Flow Explained

*User joins a room
*Browser requests camera & microphone access
*RTCPeerConnection is created
*Offer/Answer (SDP) exchanged via signaling server
*ICE candidates shared
*Direct peer-to-peer media connection established
*Live audio/video stream starts 

# Signaling Events (Example)
join-room
send-offer
send-answer
send-ice-candidate
user-left

# Signaling server does NOT handle media — only connection setup.

# Screenshots
/screenshots
 ├── landing.png
 ├── join-room.png
 ├── video-call.png

# Live Demo
https://kyra-zoom-vkpr.onrender.com/

Anjali Saini
MERN Developer | Backend & Real-time systems
📍 Sonipat, Haryana
🔗 GitHub: https://github.com/ANJALI-SAIN
