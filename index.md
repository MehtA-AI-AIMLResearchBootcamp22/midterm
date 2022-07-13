<html>
    <head>
        <title>MehtA+ AI/ML Research Bootcamp '22 midterm project</title>
        <meta charset="utf-8">
        <link rel="stylesheet" href="style.css">
        <script src="index.js"></script>
    </head>
    <body>
        <div class = "center">
            <h1>MehtA+ AI/ML Research Bootcamp '22 midterm project</h1>
            <h2>Arjun, Spencer, and Yuriy</h2>
            <h3>Identifying Author of book from text.</h3>
            <p>When first attempting to solve this problem, the first question is "what really distinguishes the writing styles of men and women?" Our first thought was to do Latent Dirichlet Allocation, which categorizes text. But, we realized that since our dataset covered a specific range of topics, there would be similar categories. Therefore, LDA would not be a good idea. One instrumental finding was that on average, women use more pronouns, adverbs, and adjectives than men, which is something we could quantify and use to distinguish the documents.</p><br>
            <p> 
            Before we knew about the differences, we were complacent with just putting the whole text through a model and letting it figure it out, which worked surprisingly well, but this doesn't help the user understand what's going on and often wastes resources like energy since the computer has to calculate larger datasets that are often very sparse. So we opted to use many of the natural language processing libraries we had been taught in class to separate the text by part of speech and then to specifically give the model only the pronouns, adjectives, and adverbs.
            </p>
            <h3>View Our Code!</h3>
            <script src="https://gist.github.com/ybidochko/88ab8a9b5f0540bb9c70dfec2e8f4ab2.js"></script>
        </div>
    </body> 
</html>