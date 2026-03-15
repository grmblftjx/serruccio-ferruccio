+++
title = 'Love'
date = 2026-03-15
draft = false
+++

<ul>
  {{ range .Pages }}
    <li><a href="{{ .RelPermalink }}">{{ .Title }}</a></li>
  {{ end }}
</ul>

