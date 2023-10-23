---
layout: default
title: While Loops - Level 3
description:
---

Rearrange the lines of code so that the program will ask the user for a number, then count from that number up to 100. Look out for the extra blocks that you don't need to use!

<div id="WhileLoops-Problem3-sortableTrash" class="sortable-code"></div> 
<div id="WhileLoops-Problem3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="WhileLoops-Problem3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="WhileLoops-Problem3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "num = int(input(&quot;Enter a number: &quot;)\n" +
    "while num &lt; 100:\n" +
    "	print(num)\n" +
    "	num = num + 1\n" +
    "num = input(&quot;Enter a number: &quot;) #distractor\n" +
    "while num &gt; 100: #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "WhileLoops-Problem3-sortable",
    "max_wrong_lines": 1,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "WhileLoops-Problem3-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#WhileLoops-Problem3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#WhileLoops-Problem3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
