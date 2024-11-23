<!DOCTYPE html>
<html>
    <head>
        <title>My Cool Website</title>

        <style>
            img {
                width: 600px;
                height: auto;
            }

            h1 {
                color: red;
            }
        </style>

    </head>
    <body>
        <h1>My Cool Website</h1>
        <p>I think HTML is neat!</p>

        <img src="https://www.lectura-specs.com/models/renamed/orig/rigid-dump-truck-777-g-caterpillar.jpg">

        <blockquote>"I looked like this when I was young, and I still do." - Yogi Berra</blockquote>
        <button onclick="changeQuote()">Change Quote</button>

        <script>
            var index = 0;

            function changeQuote() {
                var quotes = [
                    `"I really like web development!" - Dave Smith-Hayes`,
                    `"I am enjoying my time at Hammer Hacks!" - Dave Smith-Hayes`,
                    `"Dumptrucks!" - My Son`,
                    `"I looked like this when I was young, and I still do." - Yogi Berra`
                ];

                var blockquote = document.querySelector("blockquote");
                blockquote.innerHTML = quotes[index];

                index++;
                if (index >= 4) {
                    index = 0;
                }
            }
        </script>
    </body>
</html>
