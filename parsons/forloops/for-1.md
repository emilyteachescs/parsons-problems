Complete the code so that it will count by 10's up to 100.
There is one block you will **not** need to use!

<div id="ForLoops-1-sortableTrash" class="sortable-code"></div> 
<div id="ForLoops-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="ForLoops-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="ForLoops-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "for x in range(10):\n" +
    "	num = x * 10\n" +
    "    print(num)\n" +
    "for x in range(100) #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "ForLoops-1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "ForLoops-1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#ForLoops-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#ForLoops-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
