---
name: PD-LED
label: Multimorphic PD-LED
manufacturer: Multimorphic
documentation_link: https://docs.missionpinball.org/hardware/multimorphic/index.html
link: https://www.multimorphic.com/
---
{% assign board = site["hardware_platforms"] | where:"name", "P3-Roc" | first %}
Dedicated parallel lights controller. Newer versions also allow serial LEDs.
Part of the <a href="{{ board.url | prepend: site.baseurl }}">{{ board.label }}</a> platform.
