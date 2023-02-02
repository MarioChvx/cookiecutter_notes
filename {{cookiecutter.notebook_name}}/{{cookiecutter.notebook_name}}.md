---
title: {{ cookiecutter.notebook_name }}
author: |
  | {{ cookiecutter.personal_name }}
date: {% now 'local', '%d/%m/%Y' %}
thanks:
{% if cookiecutter.use_math == True -%}
output:
  pdf_document:
    includes:
      in_header:
        - \usepackage{amsmath}
{% endif %}
---

\maketitle

## Text here
