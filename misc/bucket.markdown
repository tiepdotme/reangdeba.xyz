---
layout: page
title: "Bucket list"
comments: false
permalink: /bucket/
---
<p>This list was last modified on: <i>{{ page.last_modified_at | date: "%B %-d, %Y" }}</i>.</p>

### Life

<div class="container">
<div class="progress">
  <div class="progress-bar progress-bar-striped bg-danger" role="progressbar" aria-valuemin="0" aria-valuemax="100" id="lifeprogressbar"></div>
</div>
</div>

> Things I wish to do before I die.

### Progress
<div class="container">
<div class="progress">
  <div class="progress-bar progress-bar-striped bg-success" role="progressbar" aria-valuemin="0" aria-valuemax="100" id="theprogressbar"></div>
</div>
</div>

4.  Go camping
9.  Start a company
10. <s>Take a train journey</s>
11. <s>Meet Stephen Hawking.</s>
12. <s>Meet HC Verma</s>
13. Learn to play the Guitar
14. Visit Disneyland
15. Give TED talk
16. Visit Googleplex
17. Visit Apple Park
18. Take a selfie outside the Taj Mahal
19. Go on a hike
20. Take a hot air balloon ride
21. Go scuba diving
22. Fly an airplane
23. Meet Hasan Minhaj
24. <s>Perform at an open mic</s>
27. Graduate from college
28. Get a PhD
29. Learn Korean
31. Meet Prof. David J. Malan
32. Start a not-for-profit organisation
33. Sing in front of an audience
40. Skydive
41. Christmas in New York
42. Move to Seoul
43. Be a commencement speaker
44. Masters degree in CS
1. Get my eyebrows done in Dubai
2. Visit Bhutan
3. Eat local food in Tehran
4. Take a train to Saint Petersburg
5. Travel through Kashmir
28. Read 100 books
6. Live in Singapore
7. Go on a African Safari
8. Attend Tomorrowland
10. Take underwater photos in Maldives
11. Watch Real Madrid play
12. Visit Old Trafford
13. Get blue hair dye in China
14. Pose in front of the Pyramids in Egypt
15. Post sunset pictures of Auckland, New Zealand
17. Never get "high"
18. Donate 10% of my income each year
19. Publish before finishing undergraduate degree

<blockquote><p>For suggestions please send me an <a href="mailto:hi@reangdeba.xyz">email</a>, or reach out on <a
        target="_blank" href="https://twitter.com/reangdeba">Twitter</a>.</p></blockquote>

<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
        integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
        crossorigin="anonymous"></script>

<script>
        var newprogress = Math.round(4/46*100);
$('#theprogressbar').attr('aria-valuenow', newprogress).css('width', newprogress+'%');

$('#theprogressbar').text(newprogress + '%');
</script>

<script>
        var progress = Math.round(21/92*100);
$('#lifeprogressbar').attr('aria-valuenow', progress).css('width', progress+'%');

$('#lifeprogressbar').text(progress + '%');
</script>
