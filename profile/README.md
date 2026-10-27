# VisionVend

Retrofit hardware that turns the case you already own into a secure,
cashier-less store — not a classic vending machine.

VisionVend is not tied to drinks, snacks, or gas stations. The kit turns a
display fridge, a merchandiser, an open shelf, or a storefront case into an
unattended storefront that sells anything, anywhere, at any hour. A case
outside a hardware store can sell light bulbs; a case in front of a grocery
store can sell milk, butter, cheese, and eggs at 3am; a mall-corridor case
keeps selling after the stores around it close; a dorm case can stock
personal care. If a store sells it, a VisionVend case can sell it after that
store closes.

## What we build

- **Cashier-less retrofit kit** — cameras, compute, and locking that drop into
  standard display fridges and other cases. No new cooler required.
- **SKU onboarding pipeline** — iPhone turntable capture (video + `yaw.jsonl`
  manifest) feeds the product-recognition models.
- **Synthetic data & simulation** — Isaac Sim digital twin generates training
  data and person-ReID trajectories before real-world deployment.

**Pricing:** $49/month per kit + $0.10 per SKU (as of 2026-10-26).

## Repositories

Table verified against the org repo list on 2026-10-26.

| Repo | What it is |
|---|---|
| [VisionVend](https://github.com/VisionVend/VisionVend) | Main monorepo — iOS apps (editor, retailer, customer), hardware, ML |
| [MusePi](https://github.com/VisionVend/MusePi) | Pi hub monitor: Hailo/GPU/USB/HDMI/network monitor with web dashboard and SwiftUI iOS/macOS client |
| [vv-capture](https://github.com/VisionVend/vv-capture) | iPhone 3D scanning for product onboarding |
| [vision-vend.com](https://github.com/VisionVend/vision-vend.com) | Interactive 3D product demo — the homepage is a first-person Three.js simulation of the VisionVend cashier-less machine |
| [visionvend-sim](https://github.com/VisionVend/visionvend-sim) | Isaac Sim digital twin: synthetic data + policy trajectories |
| [isaac-reid-pipeline](https://github.com/VisionVend/isaac-reid-pipeline) | Synthetic-retail person ReID: YOLO → ByteTrack → TransReID + FAISS |
| [retail-786k-trainer](https://github.com/VisionVend/retail-786k-trainer) | Retail-786k dataset + baseline training console |
| [visionvend-cam](https://github.com/VisionVend/visionvend-cam) | Camera firmware for XIAO ESP32-S3 Sense (historical Wi-Fi/SD/REST/MJPEG/OTA firmware, kept for reference; no live successor has been confirmed) |
| [xiao-uvc](https://github.com/VisionVend/xiao-uvc) | UVC + CDC webcam firmware for XIAO ESP32-S3 (bench tooling) |
| [ArducamBridge](https://github.com/VisionVend/ArducamBridge) | Camera-ops stack: Pi Zero 2 WH MJPEG bridge + native macOS/iOS clients + Mac vision workbench |
| [poor-mans-motion-detection](https://github.com/VisionVend/poor-mans-motion-detection) | Frame-differencing motion detection CLI + browser GUI |
| [visionvend-sketchfab](https://github.com/VisionVend/visionvend-sketchfab) | Sketchfab 3D model library / catalog for VisionVend products and scenes |
| [visionvend-cooler-fleet](https://github.com/VisionVend/visionvend-cooler-fleet) | Companion media/pipeline repo for the merchandising-cooler fleet |
| [ui-editor](https://github.com/VisionVend/ui-editor) | Single-file UI editor for iOS app screen galleries (historical copy); live tool moved to [VisionVend/tools/ui-editor](https://github.com/VisionVend/VisionVend/tree/main/VisionVend/tools/ui-editor) in the monorepo |

## About this profile

This repo is currently **private**, so this README does not render on the
public VisionVend organization profile page: GitHub renders a public org
profile README only from a **public** `.github` repo, and a member-only
README only from a **private `.github-private`** repo. A private `.github`
repo is neither. Whether this profile should go public or move to
`.github-private` is a decision for  (see
`archived-and-github-FIXES-2026-10-26.md` in the fix workspace) — the
visibility has deliberately not been changed here.

Org-wide defaults live in this repo's root: `CONTRIBUTING.md`,
`CODE_OF_CONDUCT.md`, `SECURITY.md`, `LICENSE-GUIDANCE.md`, and the
issue/PR templates under `.github/`. They apply to org repos that do not
define their own; a repo's own files always take precedence.

## Contact

- Email: info@vision-vend.com
- Phone: 
- Built by [coresapian inc](https://coresapian.com), , 
