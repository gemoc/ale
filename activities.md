---
layout: page
title: Activities
permalink: /activities/
order: 2
---

<link rel="stylesheet" href="{{ site.baseurl }}/css/all.css">

Here is the timeline of the meetings and visits organized in the context of ALE:

{% include jekyll-timeline.html 
    startYear=2017
    timelineHeight=600  
    col1Title="Meetings of the ALE team" col1Events=site.data.meetings
    col2Title="Visits of the ALE researchers" col2Events=site.data.visits %}