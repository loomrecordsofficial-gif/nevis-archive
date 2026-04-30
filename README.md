<!DOCTYPE html>
<html>
<head>
<title>archive_01</title>
</head>

<body style="background:black; color:#cfcfcf; font-family:monospace; padding:40px;">

<p>> loading archive...</p>
<p>> file unstable</p>
<p>> attempting recovery...</p>

<br>

<p>ARCHIVE: A01</p>
<p>> integrity: 63%</p>

<br>

<p>[log_01] playback initiated</p>
<p>[log_02] identity mismatch detected</p>

<br>

<p>> input required</p>

<input type="text" id="pw">
<button onclick="check()">enter</button>

<p id="result"></p>

<p style="opacity:0.2;">still watching</p>

<script>
function check(){
  let input = document.getElementById("pw").value;

  if(input === "replay_again_dont"){
    document.getElementById("result").innerHTML = "> access granted...";

    setTimeout(()=>{
      window.location.href = "archive_02.html";
    }, 1000);

  } else {
    document.getElementById("result").innerHTML = "> access denied";
  }
}
</script>

</body>
</html>
