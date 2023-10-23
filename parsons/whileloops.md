# While Loops - Testing

## Problem 1
<div id="Testing 1-sortableTrash" class="sortable-code"></div> 
<div id="Testing 1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="Testing 1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="Testing 1-newInstanceLink" value="Reset Problem" type="button" /> 
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
    "sortableId": "Testing 1-sortable",
    "max_wrong_lines": 1,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "Testing 1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#Testing 1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#Testing 1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Problem 2
Just another problem
