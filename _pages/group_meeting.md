---
title: "Group meeting"
layout: textlay
excerpt: "Group meeting"
sitemap: false
permalink: /group_meeting/
---

## Group meeting and Journal Club Schedule

Group meetings are held every other week and journal club is held every week.

The normal time/place for group meetings and journal club is Tues. 14:00-16:00 in 715 rom.

The normal time/place for Joint Journal Club is Mon.19:00 online, please [login in](https://cvirlab.quickconnect.cn/#/signin) to check the previous culb videos. 

<b>Schedule is subject to change, please check frequently. </b>

<div class="row">
<div class="col-sm-6 clearfix">

### Group meeting

{% for meeting in site.data.seminar %}
  <b>{{ meeting.date}}</b>  {{ meeting.presenter}}
  <br /> 

{% endfor %}

</div>
  
<div class="col-sm-6 clearfix">
### Journal club
{% for journal in site.data.journal_club %}
  <b>{{ journal.date}}</b>  {{ journal.presenter}}
  <br /> 

{% endfor %}
</div>
</div>
