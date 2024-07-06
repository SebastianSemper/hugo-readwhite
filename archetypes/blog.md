+++
title = "{{ replace .Name "-" " " | title }}"
date = "{{time.Format .Site.Params.dateformat .Date }}"

menu = "main"

tags = [{{ range $plural, $terms := .Site.Taxonomies }}{{ range $term, $val := $terms }}"{{ printf "%s" $term }}",{{ end }}{{ end }}]
+++