{% include '_markbind/layouts/css.md' %}
{% include '_markbind/layouts/header.md' %}
{% set file =  "" if te3201 else "admin" %}
{% set sitenav_title =  "Admin info" %}
{% include '_markbind/layouts/body.md' %}
{% include '_markbind/layouts/footer.md' %}