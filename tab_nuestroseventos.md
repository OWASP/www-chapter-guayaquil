---
title: nuestroseventos
displaytext: Nuestros Eventos
layout: null
tab: true
order: 4
tags: front-matter
---

## Nuestros Eventos

Hemos organizado mutliples conferencias en disitintas universidades de Guayaquil. Pero aun faltan mas.

Preparense que aun fatan los mejores eventos

### Mantente al tanto de nuestros futuros eventos en Meetup:
{% include chapter_events.html group=page.meetup-group %}

<script type='text/javascript'>
  $(function(){
    $(".timeclass").hover(function() {
      utc_str = $(this).text();
      ndx = utc_str.indexOf(':');
      st_hour_str = utc_str.substring(0, ndx);
      st_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(st_hour_str), parseInt(st_min_str), 0);
      start_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);

      ndx = utc_str.lastIndexOf(':');
      end_hour_str = utc_str.substring(ndx - 2, ndx - 1);
      end_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(end_hour_str), parseInt(end_min_str), 0);
      end_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);
      popstr = start_dt.toLocaleString(luxon.DateTime.TIME_WITH_SECONDS) + ' to ' + end_dt.toLocaleString(luxon.DateTime.TIME_WITH_SHORT_OFFSET);
      $(this).prop('title', popstr);
    });
  });

  
</script>



### Date una vuelta por nuestra cuenta de Twitter para estar actualizado con nuestras publicaciones

<div class="container" style="width:500px;margin: auto;"><a class="twitter-timeline" href="https://twitter.com/Owasp_Guayaquil?ref_src=twsrc%5Etfw">Tweets by Owasp_Guayaquil</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></div>
