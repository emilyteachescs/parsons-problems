---
layout: default
title: While Loops - Testing
---

## Problem 1
<div id="Testing1-sortableTrash" class="sortable-code"></div> 
<div id="Testing1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="Testing1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="Testing1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "number = int(input(&quot;Enter a number: &quot;))\n" +
    "if number &gt; 10:\n" +
    "	print(&quot;Greater than 10&quot;)\n" +
    "else:\n" +
    "	print(&quot;Less than 10&quot;)\n" +
    "number = input(&quot;Enter a number&quot;) #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "Testing1-sortable",
    "max_wrong_lines": 1,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "Testing1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shufffleLines();
  $("#Testing1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#Testing1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Problem 2
Just another problem
<div id="MaybeThis-sortableTrash" class="sortable-code"></div> 
<div id="MaybeThis-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="MaybeThis-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="MaybeThis-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;Simpler test&quot;)\n" +
    "print(&quot;Please work&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "MaybeThis-sortable",
    "max_wrong_lines": 0,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "MaybeThis-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#MaybeThis-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#MaybeThis-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Problem 3
<div id="p1-sortableTrash" class="sortable-code"></div>
<div id="p1-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="p1-feedbackLink" value="Get Feedback" type="button" />
    <input id="p1-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
  var initial = "print(\"Hello\")\n" +
    "print(\" \")\n" +
    "print(\"World\")\n" +
    "print(\"!\")";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "p1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en",
    "trashId": "p1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#p1-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#p1-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
</script>

# Problem 4
Testing a simple one
<div id="NextTest-sortableTrash" class="sortable-code"></div> 
<div id="NextTest-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="NextTest-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="NextTest-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
  var initial = "print(&quot;Simpler test&quot;)\n" +
    "print(&quot;Please work&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "NextTest-sortable",
    "max_wrong_lines": 1,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "NextTest-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#NextTest-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#NextTest-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
</script>
