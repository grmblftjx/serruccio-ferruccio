+++
title = 'Love'
date = 2026-03-15
draft = false
+++

<ul>
{{ range .Pages.ByWeight }}
  <li>{{ .Title }}</li>
{{ end }}

{{ range .Sections.ByWeight }}
  <li>{{ .Title }}
    <ul>
      {{ range .Pages.ByWeight }}
        <li>{{ .Title }}</li>
      {{ end }}
      
      {{ range .Sections.ByWeight }}
        <li>{{ .Title }}
          <ul>
            {{ range .Pages.ByWeight }}
              <li>{{ .Title }}</li>
            {{ end }}
          </ul>
        </li>
      {{ end }}

    </ul>
  </li>
{{ end }}
</ul>
