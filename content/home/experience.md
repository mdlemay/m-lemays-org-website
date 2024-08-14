---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: experience

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 40

title: Experience
subtitle:

# Date format for experience
#   Refer to https://wowchemy.com/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` items below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
experience:
  - title: Senior Staff Research Scientist
    company: Intel Labs
    company_url: 'https://www.intel.com/content/www/us/en/research/overview.html'
    company_logo: ''
    location: Oregon
    date_start: '2012-06-04'
    date_end: ''
    description: |2-
        My research has generated or influenced hardware and software security architectures
        deployed on a large proportion of computer systems in use today.

        I have contributed to shipping processor security technologies, including
        [Control-Flow Enforcement Technology (CET)](https://www.forbes.com/sites/tonybradley/2020/06/17/intel-cet-raises-the-bar-for-malware-defense/) and
        [VT-Redirect Protection (VT-rp)](https://www.pcworld.com/article/619047/intels-12th-gen-vpro-chips-now-actively-fight-ransomware-supply-chain-attacks.html).

        Principal Investigator for [Intel's project on Cryptographic Capability Computing (C3)](https://www.intel.com/content/www/us/en/newsroom/news/intel-and-ucsd-join-darpa-cyberdefense-program.html) in the [DARPA HARDEN program](https://www.darpa.mil/news-events/2022-10-13).

        I [designed](https://groups.google.com/a/chromium.org/g/memory-safety-dev/c/PDi1cvAvUGc)
        and [co-developed](https://groups.google.com/a/chromium.org/g/memory-safety-dev/c/1tYGORldm3w)
        deterministic spatial safety support for MiraclePtr in the Chrome browser.

        My LLVM-based research on shielding stack memory from corruption helped lead to a 2022
        paper in a top-tier programming languages conference
        [covered by ZDNet](https://www.zdnet.com/article/this-new-firefox-browser-feature-could-stop-zero-day-bugs-in-their-tracks/).

        I also researched approaches for scalable isolation, e.g., using [segmentation to accelerate WebAssembly](https://plas2022.github.io/files/pdf/SegueColorGuard.pdf) (upstreamed in [wasm2c](https://github.com/WebAssembly/wabt/pull/2395)).

  - title: PhD Student and Postdoc
    company: University of Illinois at Urbana-Champaign
    company_url: 'http://seclab.illinois.edu/'
    company_logo: ''
    location: Illinois
    date_start: '2005-09-01'
    date_end: '2012-05-15'
    description: |2-
        Advisor: [Carl A. Gunter](http://cgunter.cs.illinois.edu/)

        National Defense Science and Engineering Graduate (NDSEG) Fellow

        PhD Dissertation: [Compact Integrity-Aware Architectures](http://hdl.handle.net/2142/26037)

        MS Thesis: [Dependable Emergency-Response Networking Based on Retaskable Network Infrastructures](http://seclab.illinois.edu/wp-content/uploads/2011/03/LeMayMSThesis.pdf)

        TA for Advanced Computer Security (Instructor: Carl A. Gunter)

        TA for Advanced Operating Systems (Instructor: Samuel T. King)


design:
  columns: '2'
---
