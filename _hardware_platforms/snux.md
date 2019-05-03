---
name: Snux
label: Snux System 11
manufacturer: Snux
documentation_link: http://docs.missionpinball.org/en/latest/hardware/snux/
link:
---
{% assign board = site["hardware_platforms"] | where:"name", "P-Roc" | first %}

Adaptor board to connect a <a href="{{ board.url | prepend: site.baseurl }}">{{ board.label }}</a> to a System 11 machine.
