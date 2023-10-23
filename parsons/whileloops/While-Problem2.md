---
layout: default
title: While Loops - Problem 2
description: 
---

Put the lines of code in the correct order so that the code will print the numbers 1 - 9. 

<div id="WhileLoops-Problem2-sortableTrash" class="sortable-code"></div> 
<div id="WhileLoops-Problem2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="WhileLoops-Problem2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="WhileLoops-Problem2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "num = 1\n" +
    "while num &lt; 10:\n" +
    "	print(num)\n" +
    "	num = num + 1";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "WhileLoops-Problem2-sortable",
    "max_wrong_lines": 1,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "WhileLoops-Problem2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#WhileLoops-Problem2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#WhileLoops-Problem2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
