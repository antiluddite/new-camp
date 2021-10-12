
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
$(document).ready(function(){
  $(".btn-false").click(function(){
    $("#btnShowBanana").collapse("show");
  });
});


$(document).ready(function(){
  $("#btnShowBanana").click(function(){
    $(".collapse").collapse('show');
  });
  $("#btnHideBanana").click(function(){
    $(".collapse").collapse('hide');
  });
    $("#btnShowMonkey").click(function(){
    $(".collapse").collapse('show');
  });
  $("#btnHideMonkey").click(function(){
    $(".collapse").collapse('hide');
  });
  
});