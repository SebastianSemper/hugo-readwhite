+++
title = "{{ replace .Name "-" " " | title }}"
date = "{{time.Format .Site.Params.dateformat .Date }}"
+++