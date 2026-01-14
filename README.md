# CSS-Day-8
<!DOCTYPE html>
<html>
<head>
    <title>CSS Position and Z-Index Practice</title>

    <style>
        body {
            margin: 0;
            padding-top: 60px;
            font-family: Arial, sans-serif;
        }

        /* Fixed Header */
        .header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: #333;
            color: white;
            text-align: center;
            padding: 15px;
            z-index: 1000;
        }

        /* Relative Box */
        .relative-box {
            position: relative;
            width: 300px;
            height: 150px;
            background-color: lightblue;
            margin: 40px;
            padding: 10px;
        }

        /* Absolute inside Relative */
        .absolute-box {
            position: absolute;
            top: 5px;
            right: 5px;
            background-color: orange;
            padding: 5px;
            font-size: 14px;
        }

        /* Sticky Box */
        .sticky-box {
            position: sticky;
            top: 60px;
            background-color: yellow;
            padding: 10px;
            margin: 40px;
        }

        /* Z-index Layers */
        .layer-container {
            position: relative;
            height: 150px;
            margin: 40px;
        }

        .layer1 {
            position: absolute;
            width: 150px;
            height: 100px;
            background-color: red;
            top: 20px;
            left: 20px;
            z-index: 1;
            color: white;
            padding: 5px;
        }

        .layer2 {
            position: absolute;
            width: 150px;
            height: 100px;
            background-color: green;
            top: 40px;
            left: 60px;
            z-index: 2;
            color: white;
            padding: 5px;
        }

        /* Space for scrolling */
        .space {
            height: 800px;
        }
    </style>
</head>

<body>

    <div class="header">
        Fixed Header at Top
    </div>

    <div class="relative-box">
        Relative Box
        <div class="absolute-box">
            Absolutely Positioned (Top Right)
        </div>
    </div>

    <div class="sticky-box">
        I stick when scrolling
    </div>

    <div class="layer-container">
        <div class="layer1">Layer 1</div>
        <div class="layer2">Layer 2 (on top)</div>
    </div>

    <div class="space"></div>

</body>
</html>
