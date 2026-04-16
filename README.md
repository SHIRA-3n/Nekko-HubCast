# Nekko-HubCast

Local desktop application for YouTube live streaming creators.

## Overview

Nekko-HubCast enables streamers to receive their own YouTube live chat
messages with low latency, trigger AI character responses, and display
chat overlays — all processed locally on the user's PC.

## Features

- Real-time YouTube live chat reception via `liveChatMessages.streamList` (gRPC)
- Local AI-driven auto-response generation
- Stream overlay display
- Local chat log storage and analytics

## Architecture

- **Client-local only.** No third-party server involved.
- Each user provides their own Google Cloud API key.
- All data (chat logs, AI memory) stored in the user's IndexedDB.

## Status

In development. Future release planned as a downloadable desktop
application (via Electron). Currently operated privately by the developer.

## Privacy

All YouTube data handled by this application stays on the user's local
machine. See the [Privacy Policy](https://gist.github.com/SHIRA-3n/xxxxx)
for details.

## Technology Stack

- TypeScript / React / Vite
- Node.js / Express / WebSocket
- @grpc/grpc-js for YouTube gRPC Server Streaming
- IndexedDB (Dexie) for local storage

## Compliance

This application adheres to the
[YouTube API Services Terms of Service](https://developers.google.com/youtube/terms/api-services-terms-of-service)
and the
[YouTube Developer Policies](https://developers.google.com/youtube/terms/developer-policies).

## Contact

Developer: SHIRA (k.shira07@gmail.com)
