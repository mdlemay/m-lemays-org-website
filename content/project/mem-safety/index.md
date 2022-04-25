---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Memory safety with no additional metadata"
summary: "The Chromium team has developed BackupRefPtr, which seeks to deterministically enforce temporal memory safety.
  I developed an extension to BackupRefPtr to also deterministically enforce spatial memory safety (e.g., to mitigate buffer overflows).
  It does not require storing any additional metadata beyond what the underlying allocator already uses, although it is stateful due to needing the allocator metadata to be loaded during spatial safety checks.
  It operates by checking that the pointer stays within valid bounds any time the pointer is updated."
authors: [admin]
tags: []
categories: []
date: 2021-03-04

# Optional external URL for project (replaces project detail page).
external_link: "https://groups.google.com/a/chromium.org/g/memory-safety-dev/c/PDi1cvAvUGc"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
