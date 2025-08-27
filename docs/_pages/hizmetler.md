---
title: "Hizmetler"
permalink: /hizmetler/
layout: single
classes: wide
---

{% include feature_row id="hizmetler" type="left" %}

{% capture hizmet1 %}
**Akademik Analiz:** Tez-makale istatistiği, örneklem hesaplama, metodoloji danışmanlığı.
{% endcapture %}
{% capture hizmet2 %}
**Kurumsal Analiz:** KPI, A/B test, BI panoları, pazar segmentasyonu.
{% endcapture %}
{% capture hizmet3 %}
**Eğitim & Mentorluk:** R, Python, SPSS eğitimleri; kod gözden geçirme.
{% endcapture %}

{% assign feature_row = site.data.features.hizmetler | default: 
  ( 
    ( site.data.features.hizmetler or
      [{'title':'Akademik Analiz','excerpt':hizmet1},
       {'title':'Kurumsal Analiz','excerpt':hizmet2},
       {'title':'Eğitim & Mentorluk','excerpt':hizmet3}]
    )
  )
%}
