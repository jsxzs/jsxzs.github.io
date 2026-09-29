# LIFT project page

Project page of *LIFT: Layout-In-Future Video Generation under Large Viewpoint Change via On-Policy Self-Distillation*
(Nerfies template, same layout as `../sa4d`).

- `index.html` is edited directly. `LIFT-CAM/camlayout/cc_workstation/video_demo_build/build_project_page.py` only
  refreshes the Video Results data inside it (video paths, captions, ground-truth boxes of the conditioned objects,
  example order); `--fresh` would rebuild the page from `project_page_template.html` and discard hand edits.
- `static/videos/exNN_demoDD/{gt,ours,gen3c,uni3c,magicmotion,dav}.mp4` are the Video Results clips (640x352),
  copied from `code/video_demo/videos`.
- `static/videos/overview.mp4` is the TL;DR video (`code/LIFT_teaser_ex15.mp4`, made by
  `LIFT-CAM/camlayout/cc_workstation/teaser_video` from project-page Example 15); poster `static/images/overview_poster.jpg` (1.6 s).
- `static/videos/ui_demo.mp4` is the User Interface recording with the browser bar cropped out: made from
  `LIFT-CAM/camlayout/demo/ui_recording/LIFT_UI_Demo_60fps.mp4` (1960x1080) by cropping rows 42-1037 of frames
  0-1765 (black strips) and rows 84-1079 of frames 1766-4245 (Chrome tab strip + address bar) to 1960x996, CRF 28;
  poster `static/images/ui_poster.jpg` (6 s).
- `static/images/*` also holds the paper figures rasterised from `LIFT_paper/figs/*.pdf` (teaser, data pipeline,
  architecture, OPSD), `hf-logo.svg` and `thumbs/exNN.jpg` (ground-truth last frames for the carousel strip).
- `static/css`, `static/js` are copies of the site's shared Nerfies assets.
