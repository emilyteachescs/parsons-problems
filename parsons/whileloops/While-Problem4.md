---
layout: default
title: While Loops - Level 4
---

Arrange the lines of code so that the program will ask the user to enter the secret password. If the password is not "computerscience" then it should prompt them to try again until they enter the correct password. 


<div id="WhileLoops-Problem4-sortableTrash" class="sortable-code"></div> 
<div id="WhileLoops-Problem4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="WhileLoops-Problem4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="WhileLoops-Problem4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "password = input(&quot;What&#039;s the secret password? &quot;)\n" +
    "while password != &quot;computerscience&quot;:\n" +
    "	print(&quot;Wrong!&quot;)\n" +
    "    password = input(&quot;Try again: &quot;)\n" +
    "while password == &quot;computerscience&quot;: #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "WhileLoops-Problem4-sortable",
    "max_wrong_lines": 1,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "WhileLoops-Problem4-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#WhileLoops-Problem4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#WhileLoops-Problem4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
