### {{ title }} <sup>c</sup>
Property | Value
--- | ---
IRI | `{{ uri }}`
{%- if description is not none %}
Description | {{ description }}
{%- endif %}
{%- if scopeNote is not none %}
Usage Note | {{ scopeNote }}
{%- endif %}
{%- if supers|length > 0 %}
Super-classes | {%- for super in supers %}{{ super }}<br />{%- endfor %}
{%- endif %}
{%- if supers|length > 0 %}
Restrictions | {%- for restriction in restrictions %}{{ restriction }}<br />{%- endfor %}
{%- endif %}
{%- if supers|length > 0 %}
Sub-classes | {%- for sub in subs %}{{ sub }}<br />{%- endfor %}
{%- endif %}
{%- if in_domain_of|length > 0 %}
In domain of | {%- for i in in_domain_of %}{{ i }}<br />{%- endfor %}
{%- endif %}
{%- if in_domainIncludes_of|length > 0 %}
In domain of | {%- for i in in_domainIncludes_of %}{{ i }}<br />{%- endfor %}
{%- endif %}
{%- if in_range_of|length > 0 %}
In range of | {%- for i in in_range_of %}{{ i }}<br />{%- endfor %}
{%- endif %}
{%- if in_rangeIncludes_of|length > 0 %}
In range of | {%- for i in in_rangeIncludes_of %}{{ i }}<br />{%- endfor %}
{%- endif %}
