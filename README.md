<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Holiday Plan Confirmation</title>
    <style>
        body {
            background-color: #2b2b2b; /* Dark background color */
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            text-align: center;
            color: #ffffff; /* White text color */
        }
        .container {
            max-width: 800px;
            margin: 50px auto;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);
            background-color: #4a235a; /* Deep purple background color */
        }
        h1 {
            color: #ff69b4;
            font-size: 36px;
            margin-bottom: 30px;
        }
        button {
            padding: 12px 24px;
            margin: 10px;
            font-size: 18px;
            cursor: pointer;
            background-color: #ff69b4;
            border: none;
            color: #ffffff;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }
        button:hover {
            background-color: #ff4081;
        }
        .image-container {
            display: flex;
            justify-content: center;
            margin-top: 30px;
        }
        .image-container img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Hey kello we still on for the holiday plan??</h1>
        <h4> just send a screenshot after you click a box.</h4>
        <button id="yesButton" onclick="celebrate()">Yes</button>
        <button id="noButton" onclick="disappoint()">No</button>
        <div class="image-container">
            <div id="celebrate" class="celebrate" style="display: none;">
                <img src="https://media.giphy.com/media/3ohhwLFSZmcGZ77vxe/giphy.gif" alt="Celebration">
            </div>
            <div id="disappoint" class="disappoint" style="display: none;">
                <img src="https://media.giphy.com/media/S3Ot3hZ5bcy8o/giphy.gif" alt="Disappointment">
            </div>
        </div>
    </div>

    <script>
        function celebrate() {
            document.getElementById("celebrate").style.display = "block";
            document.getElementById("disappoint").style.display = "none";
        }

        function disappoint() {
            document.getElementById("celebrate").style.display = "none";
            document.getElementById("disappoint").style.display = "block";
        }
    </script>
</body>
</html>
