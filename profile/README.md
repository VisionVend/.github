# VisionVend

Retrofit hardware that turns the merchandiser cooler you already own into a
secure, cashier-less vending machine.

## What we build

- **Cashier-less retrofit kit** — cameras, compute, and locking that drop into
  standard display fridges. No new cooler required.
- **SKU onboarding pipeline** — iPhone turntable capture (video + `yaw.jsonl`
  manifest) feeds the product-recognition models.
- **Synthetic data & simulation** — Isaac Sim digital twin generates training
  data and person-ReID trajectories before real-world deployment.

**Pricing:** $49/month per kit + $0.10 per SKU.

## Repositories

| Repo | What it is |
|---|---|
| [VisionVend](https://github.com/VisionVend/VisionVend) | Main monorepo — iOS apps (editor, retailer, customer), hardware, ML |
| [vv-capture](https://github.com/VisionVend/vv-capture) | iPhone 3D scanning for product onboarding |
| [vision-vend.com](https://github.com/VisionVend/vision-vend.com) | Marketing site — [vision-vend.com](https://vision-vend.com) |
| [visionvend-sim](https://github.com/VisionVend/visionvend-sim) | Isaac Sim digital twin: synthetic data + policy trajectories |
| [isaac-reid-pipeline](https://github.com/VisionVend/isaac-reid-pipeline) | Synthetic-retail person ReID: YOLO → ByteTrack → TransReID + FAISS |
| [retail-786k-trainer](https://github.com/VisionVend/retail-786k-trainer) | Retail-786k dataset + baseline training console |
| [visionvend-cam](https://github.com/VisionVend/visionvend-cam) | Camera firmware for XIAO ESP32-S3 Sense |
| [xiao-uvc](https://github.com/VisionVend/xiao-uvc) | UVC + CDC webcam firmware for XIAO ESP32-S3 (bench tooling) |
| [ArducamBridge](https://github.com/VisionVend/ArducamBridge) | Camera bridge streaming from Pi Zero 2 WH + Arducam |
| [poor-mans-motion-detection](https://github.com/VisionVend/poor-mans-motion-detection) | Frame-differencing motion detection CLI + browser GUI |
| [ui-editor](https://github.com/VisionVend/ui-editor) | Single-file UI editor for iOS app screen galleries |

## Contact

- Email: info@vision-vend.com
- Phone: 
- Built by [coresapian inc](https://coresapian.com), , 
