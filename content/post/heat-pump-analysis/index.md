---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Adding a heat pump alongside a natural gas furnace"
subtitle: ""
summary: ""
authors: []
tags: []
categories: []
date: 2022-04-04
lastmod: 2022-04-04
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
#image:
#  caption: "Ladybug on fennel blossom"
#  focal_point: "Smart"
#  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
I recently replaced our 30-year old air conditioner with an air-source heat pump.

It mostly went smoothly, except that I noticed it could only run for six or seven minutes at a time, and it made loud hissing and gurgling sounds as it was about to shutdown. This is known as "short-cycling." The HVAC company sent out a technician who measured the coolant pressures as the heat pump was operating, and he determined that the pressures were far too high. He had to remove a substantial amount of coolant to bring the pressures into the proper range. He noted that since we have a very short run of copper tubing between our heat pump and HVAC system, even the coolant that came pre-charged in the heat pump may have been excessive. Since he adjusted the pressure, the heat pump has been working well.

Since I kept our high-efficiency natural gas furnace as well, that required me to decide a temperature threshold for switching between the dual fuel options (natural gas and electricity). See https://github.com/mdlemay/heat-pump-analysis/blob/main/heat-pumps.ipynb for more on that.
