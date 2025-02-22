---
# Display name
title: Michael LeMay

# Name pronunciation (optional)
#name_pronunciation: Michael LeMay

# Full name (for SEO)
first_name: Michael
last_name: LeMay

# Status emoji
#status:
#  icon: ☕️

# Is this the primary user of the site?
superuser: true

# Highlight the author in author lists? (true/false)
highlight_name: true

# Role/position/tagline
role: Senior Staff Research Scientist

# Organizations/Affiliations to display in Biography blox
organizations:
- name: Intel Labs
  url: https://www.intel.com/content/www/us/en/research/overview.html

# Social network links
# Need to use another icon? Simply download the SVG icon to your `assets/media/icons/` folder.
profiles:
  - icon: at-symbol
    url: 'mailto:m.lemay.us@ieee.org'
  - icon: brands/x
    url: https://x.com/lemaymd
  - icon: academicons/google-scholar  # Alternatively, use `graduation-cap` icon from `fab` icon pack
    url: https://scholar.google.com/citations?user=c7kQkOQAAAAJ
  - icon: brands/github
    url: https://github.com/mdlemay
  - icon: brands/linkedin
    url: https://www.linkedin.com/in/lemaymd/
  - icon: academicons/orcid
    url: https://orcid.org/0000-0001-6206-9642
  - icon: rss
    link: index.xml

# Short bio (displayed in user profile at end of posts)
bio: "Views expressed are my own and do not necessarily represent those of my employer. #IamIntel"

interests:
- Memory safety
- Anti-malware
- Computer architecture
- Compilers
- Browsers
- Formal methods
- Operating systems and virtualization

education:
  - area: M.S. & Ph.D. in Computer Science
    institution: University of Illinois at Urbana-Champaign
    #date_start: 2005-08-24
    date_end: 2011-08-08 # approximate date
    summary: |
      Advised by [Prof. Carl A. Gunter](http://cgunter.cs.illinois.edu/).

      [National Defense Science and Engineering Graduate (NDSEG) Fellow](https://web.archive.org/web/20090412061630/http://www.uwec.edu/newsreleases/highlights/041305LeMay.htm).

      M.S. Thesis: [Dependable Emergency-Response Networking Based on Retaskable Network Infrastructures](http://seclab.illinois.edu/wp-content/uploads/2011/03/LeMayMSThesis.pdf).

      Postdoc through May 2012.
    button:
      text: 'Ph.D. Dissertation (Compact Integrity-Aware Architectures)'
      url: 'https://www.ideals.illinois.edu/items/26240'
  - area: B.S. in Computer Science
    institution: University of Wisconsin-Eau Claire
    #date_start: 2000-09-05
    date_end: 2005-05-21
    summary: |
      UWEC Outstanding CS Senior of the Year, 2005

      Karlgaard Scholarship

      Summa cum laude

      National Merit Scholarship Finalist

work:
  - position: Senior Staff Research Scientist
    company_name: Intel Labs
    company_url: 'https://www.intel.com/content/www/us/en/research/overview.html'
    company_logo: ''
    location: Oregon
    date_start: '2012-06-04'
    date_end: ''
    summary: |
      My research has generated or influenced hardware and software security architectures
      deployed on a large proportion of computer systems in use today.

      I have contributed to shipping processor security technologies, including
      [Control-Flow Enforcement Technology (CET)](https://www.forbes.com/sites/tonybradley/2020/06/17/intel-cet-raises-the-bar-for-malware-defense/) and
      [VT-Redirect Protection (VT-rp)](https://www.pcworld.com/article/619047/intels-12th-gen-vpro-chips-now-actively-fight-ransomware-supply-chain-attacks.html).

      I was Principal Investigator for [Intel's project on Cryptographic Capability Computing (C3)](https://web.archive.org/web/20240917132526/https://www.intel.com/content/www/us/en/newsroom/news/intel-and-ucsd-join-darpa-cyberdefense-program.html) in the [DARPA HARDEN program](https://www.darpa.mil/news-events/2022-10-13).

      I [designed](https://groups.google.com/a/chromium.org/g/memory-safety-dev/c/PDi1cvAvUGc)
      and [co-developed](https://groups.google.com/a/chromium.org/g/memory-safety-dev/c/1tYGORldm3w)
      deterministic spatial safety support for MiraclePtr in the Chrome browser.

      My LLVM-based research on shielding stack memory from corruption helped lead to a 2022
      paper in a top-tier programming languages conference
      [covered by ZDNet](https://www.zdnet.com/article/this-new-firefox-browser-feature-could-stop-zero-day-bugs-in-their-tracks/).

      I also researched approaches for scalable isolation, e.g., using [segmentation to accelerate WebAssembly](https://plas2022.github.io/files/pdf/SegueColorGuard.pdf) (upstreamed in [wasm2c](https://github.com/WebAssembly/wabt/pull/2395)).

# DARPA HARDEN press release also archived at https://download.intel.com/newsroom/archive/2025/en-us-2023-02-01-intel-and-uc-san-diego-join-darpa-program-to-prevent-exploitation-of-computing-systems.pdf

# Skills
# Add your own SVG icons to `assets/media/icons/`
skills:
  - name: Technical Skills
    items:
      - description: App, kernel, and hypervisor development for Linux, Windows, and embedded systems with Boost and generics experience
        icon: devicon/c
      #  icon: r-project
      #  icon_pack: fab
        name: C/C++
      - name: Rust
        icon: devicon/rust
      - description: SAT/SMT solver (completed [Coursera course](https://coursera.org/verify/6ZWWW76MLMB5))
        name: SMT-LIB / Z3
      - description: Somewhat familiar with assembly language for other architectures as well
        name: X86 Assembly
      - description: Compiler framework
        name: LLVM/Clang
        icon: devicon/llvm
      - description: High-Level Synthesis (HLS) language based on Term-Rewriting Systems
        name: Bluespec SystemVerilog
      - description: Model checker based on Term-Rewriting Systems and Linear-Temporal Logic
        name: Maude
      - description: Interactive theorem prover
        name: Isabelle/HOL
      - name: Python
        icon: devicon/python
      - description: Experience using Intel Quartus and Xilinx Vivado FPGA toolchains.  Experience using Synopsys VCS and Mentor Graphics Modelsim simulators.  Experience extending and maintaining an in-house Verilog simulator during an internship with Cray, Inc.
        name: Verilog/VHDL
        icon: cpu-chip
      - description: Logic programming language
        name: Prolog
        icon: devicon/prolog

languages:
  - name: English
    percent: 100

# Awards.
#   Add/remove as many awards below as you like.
#   Only `title`, `awarder`, and `date` are required.
#   Begin multi-line `summary` with YAML's `|` or `|2-` multi-line prefix and indent 2 spaces below.
awards:
#  - title: 'Automated Reasoning: satisfiability'
#    url: https://coursera.org/verify/6ZWWW76MLMB5
#    date: '2021-01-06'
#    awarder: Coursera
#    icon: coursera
#    summary:
  - title: 'Intel Hardware Security Academic Award Honorable Mention'
    url: 'https://www.cs.utexas.edu/news/2024/shravan-narayans-innovative-research-garners-multiple-prestigious-honors-hardware'
    date: '2024-08-15'
    awarder: 'Intel'
    icon: ''
    summary: 'For Hardware-assisted Fault Isolation (HFI)'
  - title: 'IEEE MICRO Top Picks'
    url: 'https://m.lemays.org/publication/microtoppicks24/'
    date: '2024-07-09'
    awarder: 'Institute of Electrical and Electronics Engineers (IEEE)'
    icon: ''
    summary: 'For "Hardware-Assisted Fault Isolation: Going Beyond the Limits of Software-Based Sandboxing"'
  - title: 'ASPLOS Distinguished Paper'
    url: 'https://m.lemays.org/publication/asplos23/'
    date: '2023-03-25'
    awarder: '28th ACM International Conference on Architectural Support for Programming Languages and Operating Systems'
    icon: ''
    summary: 'For "Going beyond the Limits of SFI: Flexible and Secure Hardware-Assisted In-Process Isolation with HFI"'
  - title: 'ACM Senior Member'
    url: 'https://awards.acm.org/award_winners/lemay_0552118'
    date: '2022-05-02'
    awarder: 'Association for Computing Machinery (ACM)'
    icon: ''
    summary: 'Joined November 2011'
  - title: 'IEEE Senior Member'
    url: 'https://www.ieee.org/membership/senior/'
    date: '2022-06-25'
    awarder: 'Institute of Electrical and Electronics Engineers (IEEE)'
    icon: ''
    summary: 'Joined March 2013'
  - title: 'HICSS Best Paper'
    url: 'https://m.lemays.org/publication/hicss08/'
    date: '2008-01-07'
    awarder: '41st Hawaii International Conference on System Sciences'
    icon: ''
    summary: 'For "An Integrated Architecture for Demand Response Communications and Control"'
---

## About Me

Research Scientist with a focus on memory management architectures for security.
