
This is the beginning of understanding jQuery
<script>
// jQuery ready funtion/ready method from w3chools//
$(document).ready(function)

// the element selector from w3//
$(document).ready(function(){
  $("button").click(function(){
    $("p").hide();
  });
});

// jQuery click event handler//
$("p").click(function(){
  alert("The paragraph was clicked.");
});
</script>


this is a great example of a button funtion in jQuery

<!DOCTYPE html>
<html>
<head>
  <title>Twitter Bootstrap : Collapse accordion Methods using Javascript</title>
<link rel="stylesheet"
      href="http://netdna.bootstrapcdn.com/bootstrap/3.1.0/css/bootstrap.min.css">
<link rel="stylesheet"
     href="http://netdna.bootstrapcdn.com/bootstrap/3.1.0/css/bootstrap-theme.min.css">
<script src="http://code.jquery.com/jquery.min.js"></script>
<script src="http://netdna.bootstrapcdn.com/bootstrap/3.1.0/js/bootstrap.min.js"></script>
</head>
<script>
$(document).ready(function(){
    $(".btn-false").click(function(){
        $("#toggle-example").collapse({
            toggle: false
        });
    });
    $(".btn-show").click(function(){
      $("#toggle-example").collapse('show'); // show
    });
    $(".btn-hide").click(function(){
        $("#toggle-example").collapse('hide');
    });
    $(".btn-toggle").click(function(){
        $("#toggle-example").collapse('toggle');
    });
});
</script>
<style>
.DemoBS2{
    margin:20px;
}
p{
  
    padding:10px;
    margin:10px 0px;
    border:2px solid #fa4b2a;
    border-radius:10px;
    box-shadow:4px 4px 4px #ccc;
   
}

</style>
<body>
<div class="DemoBS2">
  <!-- Toogle Buttons -->
    <button type="button" class="btn btn-primary btn-false">
      Button:False</button>
     <button type="button" class="btn btn-info btn-show">
            Button:Show</button>
    <button type="button" class="btn btn-warning btn-hide">
            Button:Hide</button>
    <button type="button" class="btn btn-danger btn-toggle">
           Button:Toggle</button>
 
  <div id="toggle-example">
      <p>If you don't like something, <b>change it</b>. 
	  If you can't change it, change your <b>attitude</b>.</p>
  </div>
</div>
</body>
</html>


Terminal commands
Ctrl-c
(quit) and I use the Ctrl-c key combination for that. 
Turned out the way Ctrl-c works is quite simple — it’s just a shortcut key for sending the interrupt (terminate) signal SIGINT to the current process running in the foreground. Once the process gets that signal, it’s terminating itself and returns the user to the shell prompt.

Ctrl-z
I found another interesting and probably useful key combination Ctrl-z. This combination sends SIGTSTP signal to the process (that is running in the foreground) and basically pauses the process and returns the user to the shell prompt.

run fg %1 command
If the process is paused, there should be a way to resume it, right? And the simplest way to do it is to run fg %1 command. It will bring back the program to the foreground and continue it from the moment it was stopped at. I used it when running long unit-tests

Other commands to manage shell processes
There are some more basic shell commands to manage the processes:
ps 
  to list all the processes running on the system
jobs to list processes managed by the current shell
bg 
  to resume suspended (paused) jobs in the background
kill to send any signal to a process

As with all shell commands, the commands above accept different options that change the command behavior. For example, the processes, listed by pc, and the amount of information shown depends on the options you pass to pc command.




code pen challenge:
<!-- Update the code below this comment -->
<button id="btnShowBanana" class="btn btn-warning">Show Banana</button>

<button id="btnShowMonkey" class="btn btn-success">Show Monkey</button>

<button id="btnHideBanana"class="btn btn-warning">Hide Banana</button>

<button id="btnHideMonkey" class="btn btn-success">Hide Monkey</button>

<div>
  <img class="collapse" id="banana" src="https://i.ibb.co/82WT957/banana.png" />
  <img class="collapse" id="monkey"  src="https://i.ibb.co/VJDfnxN/monkey-w-banana.png" />
</div>
<!-- Update the code above this comment -->
<hr />
<p>This Code Challenge is intended to give you more practice with using jQuery to manipulate Bootstrap components.</p>
<p>
  For this Code Challenge, you will add code to both the HTML and JS sections of this Codepen. You will not need to update any code in the CSS section.</p>
<h3>Code Challenge</h3>
<ol>
  <li>First, add <strong>Bootstrap button classes</strong> to the buttons in the HTML section thus that the buttons have the default Bootstrap button styling and their colors match the given screenshot - the Show Banana and Hide Banana buttons should be yellow, and the Show Monkey and Hide Monkey buttons should be green.</li>
  <li>Next, add the <strong>"collapse"</strong> class to the img elements for the banana and the monkey in the HTML section. Give both img elements an <strong>id</strong> as well - <strong>"banana"</strong> and <strong>"monkey"</strong>. At this point, both the banana and monkey images should disappear.</li>
  <li>In the JS section, you will write jQuery, starting with adding the <a href="https://api.jquery.com/ready/" target="_blank">jQuery ready function/ready method</a>. You have already used the ready function in your Bootstrap course project. Refer back to the <strong>Bootstrap and jQuery Part 1</strong> exercise in your course for a reminder.</li>
  <li>Inside the ready function, you will add a <strong>jQuery selector</strong> for the button with the id of <strong>"btnShowBanana"</strong>. For an example of how to do this, refer to the <strong>"The #id Selector"</strong> section on <a href="https://www.w3schools.com/jquery/jquery_selectors.asp" target="_blank">this page</a>, or refer back to the Bootstrap and jQuery Part 1 exercise and look at how you added a jQuery selector for the element with the id of <strong>"carouselPause"</strong>.</li>
  <li>Bind the jQuery <strong>click</strong> event handler to this selector. Refer to the Bootstrap and jQuery Part 1 exercise once again for an example of how to do this. Inside the event handler, query for the banana img element using its <strong>id</strong>, then attach the <strong>.collapse("show")</strong> method to it. </li>
  <li>Add three more jQuery click event handlers: one to hide the banana when the "Hide Banana" button is clicked using the <strong>.collapse("hide")</strong> method, then two more to show and hide the monkey img in the same way.</li>
    
</ol>

<h3>Resources</h3>
<ul>
  <li><a href="https://getbootstrap.com/docs/4.5/components/buttons/" target="_blank">Bootstrap - Buttons</a></li>
  <li><a href="https://getbootstrap.com/docs/4.5/components/collapse/#collapseshow" target="_blank">Bootstrap - Collapse - JavaScript Methods</a></li>
  <li><a href="https://api.jquery.com/ready/" target="_blank">jQuery ready function</a></li>
  <li><a href="https://api.jquery.com/click/#click-handler" target="_blank">jQuery click handler</a></li>
</ul>




<script>
$(document).ready(function(){
  $("#btnShowBanana").click(function(){
    $("#banana").collapse('show');
  });
  $("#btnHideBanana").click(function(){
    $("#banana").collapse('hide');
  });
    $("#btnShowMonkey").click(function(){
    $("#monkey").collapse('show');
  });
  $("#btnHideMonkey").click(function(){
    $("#monkey").collapse('hide');
  });
});

</script>








resource for button, function, collapse, images
<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
</head>
<body>

<div class="container">
  <h2>Collapsible Methods</h2>
  <p>The toggle method toggles the collapsible content.</p>
  <p>The show method shows the collapsible content.</p>
  <p>The hide method hides the collapsible content.</p>
  <button type="button" class="btn btn-primary">Toggle</button>
  <button type="button" class="btn btn-success">Show</button>
  <button type="button" class="btn btn-warning">Hide</button> 
    
  <div class="collapse">
    Lorem ipsum dolor sit amet, consectetur adipisicing elit,
    sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
  </div>
</div>

<script>
$(document).ready(function(){
  $(".btn-primary").click(function(){
    $(".collapse").collapse('toggle');
  });
  $(".btn-success").click(function(){
    $(".collapse").collapse('show');
  });
  $(".btn-warning").click(function(){
    $(".collapse").collapse('hide');
  });
});
</script>

</body>
</html>
