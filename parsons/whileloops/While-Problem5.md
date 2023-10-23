---
layout: default
title: While Loops - Level 5
---

Rearrange the code below. Once complete, the program should ask the user for a number, print the square of that number, and then ask the user if they would like to do it again. If they say yes, the program should prompt them to enter another number, otherwise the program should print "Thank you, come again.".

<div id="WhileLoops-Problem5-sortableTrash" class="sortable-code"></div> 
<div id="WhileLoops-Problem5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="WhileLoops-Problem5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="WhileLoops-Problem5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "again = True\n" +
    "while again:\n" +
    "	number = int(input(&quot;Enter a number: &quot;))\n" +
    "	print(number * number)\n" +
    "	choice = input(&quot;Would you like to try again? Y/N &quot;)\n" +
    "	if choice != &quot;Y&quot; and choice != &quot;Yes&quot; and choice != &quot;y&quot;:\n" +
    "		again = False\n" +
    "print(&quot;Thank you, come again.&quot;)\n" +
    "    \n" +
    "	";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "WhileLoops-Problem5-sortable",
    "max_wrong_lines": 1,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "WhileLoops-Problem5-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#WhileLoops-Problem5-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#WhileLoops-Problem5-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
