<html>
    <head>
        <meta charset="utf-8">
        <title>New webpage</title>
    </head>
    <body>
    Money: <span id="money"></span><br>
    New ammount: <input id="nm">
    Password<input id="pass">
    <button onClick="change();">Apply Changes</button>
    <script>
    document.getElementById("money").innerHTML = localStorage.getItem("money");
    var money = localStorage.getItem("money");
    function change (){
        if(document.getElementById("pass").value==="44333"){
            localStorage.setItem("money",document.getElementById("nm").value);
            document.getElementById("money").innerHTML = localStorage.getItem("money");
        }}
    </script>
    </body>
</html>
