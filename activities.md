---
layout: page
title: Activities
permalink: activities.html
order: 2
---

<link rel="stylesheet" href="{{ site.baseurl }}/css/all.css">
<link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/vis/4.20.1/vis.min.css" />
<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/vis/4.20.1/vis.min.js"></script>

## Timeline 

Here is the timeline of the meetings and visits organized in the context of ALE:

<div id="visualization"></div>

<script type="text/javascript">
  // DOM element where the Timeline will be attached
  var container = document.getElementById('visualization');

  // Create a DataSet (allows two way data-binding)
  var groups = new vis.DataSet([
    {id: 1, content: 'Meetings'},
    {id: 2, content: 'Visits'}
  ]);
  
  var items = new vis.DataSet([
    {content: 'Team creation /<br>Website', start: '2017-01-01', type: 'point', group: 1},
    {content: 'Kick-off meeting', start: '2017-03-27', end: '2017-03-28', type: 'point', group: 1},
    {content: 'Visit Manuel Leduc<br>@ CWI<br>(3 weeks)', start: '2017-04-03', type: 'point', group: 2},
    {content: 'Visit Fabien Coulon<br>@ CWI<br>(1 week)', start: '2017-09-04', type: 'point', group: 2},
	  {content: 'Visit Tijs van der Storm<br>@ Toulouse<br>(3 days)', start:'2017-09-27', type:'point', group: 2},
	  {content: 'Visit Benoit Combemale<br>&amp; Olivier Barais @ CWI<br>(2 days)', start:'2017-11-02', type: 'point', group: 2}
  ]);

  // Configuration for the Timeline
  var options = {start: '2017-01-01', end: '2017-12-31'};

  // Create a Timeline
  var timeline = new vis.Timeline(container, items, groups, options);
</script>
<br/>

## Plenary meetings

-	March 27-28, 2017: Kickoff meeting at Inria Rennes, FR

## Visits

-	April XX-XX, 2017: Visit of Manuel Leduc at CWI
-	September XX-XX, 2017: Visit of Fabien Coulon at CWI
- October 26-29, 2017: Visit of Tijs v. d. Storm at Inria
- November 2-3, 2017: Visit of Benoit Combemale at CWI