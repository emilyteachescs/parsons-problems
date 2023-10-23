---
layout: default
title: While Loops - Level 1
description: 
---

Put the blocks in the correct order so that the program would print "Hello!" forever.

<div id="WhileLoops-Problem1-sortableTrash" class="sortable-code"></div> 
<div id="WhileLoops-Problem1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="WhileLoops-Problem1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="WhileLoops-Problem1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "while True:\n" +
    "	print(&quot;Hello!&quot;)\n" +
    "while: #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "WhileLoops-Problem1-sortable",
    "max_wrong_lines": 1,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "WhileLoops-Problem1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#WhileLoops-Problem1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#WhileLoops-Problem1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
