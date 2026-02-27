# internet-status-detector
This project demonstrates a simple and efficient way to detect internet connectivity in a web browser using JavaScript. It dynamically switches between online and offline views based on network status, leveraging the navigator.onLine API and browser events to provide a responsive and user-friendly experience.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <div id="box">
        <h1 id="display">Welcome To Our Website.......!</h1>
    </div>
    <h1 id="notice">No-internate</h1>
    <script>
        var aviater = document.getElementById("box");
        var notice = document.getElementById("notice");
        setInterval(cheack,10);
        function cheack(){
            if(navigator.onLine==true){
            aviater.style.display="block";
            notice.style.display="none";
        }
        else{
            aviater.style.display="none";
            notice.style.display="block";
        }
        }
    </script>
</body>
</html>
