Complete the code so that it will print each character of the name as a capital letter followed by an excalmation mark!

<div id="for-2-sortableTrash" class="sortable-code"></div> 
<div id="for-2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="for-2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="for-2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "name = &quot;Emily&quot;\n" +
    "for ch in name:\n" +
    "	shout = ch.upper() + &quot;!&quot;\n" +
    "	print(shout)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "for-2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#for-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#for-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
