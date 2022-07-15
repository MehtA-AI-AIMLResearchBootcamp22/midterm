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
            <h3>Identifying Genders of Science Authors in the 1600s.</h3>
            <p>When attempting to solve this problem, the first question is "what distinguishes the writing styles of men and women?" Our first thought was to do Latent Dirichlet Allocation, which categorizes text, but we realized that since our dataset covered a specific range of topics, there would be similar categories. Therefore, LDA would not be the most optimal strategy in this prediction. After performing tests on the data and understanding the research, we concluded that the main difference between male and female authors is that the use of pronouns is more pronounced in the works of female authors than in males. Additionally, there was a significant increase in the use of adjectives and adverbs by female authors relative to the male authors. These features are all something we could quantify and use to identify the gender of an author of a document.</p><br>
            <h3>Methods</h3>
            <p> 
            Before we were aware of the distinction, we were complacent with just putting the whole text through a model and letting it figure it out (Bag of Words), which worked surprisingly well. However, this doesn't help the user understand what's going on and often wastes resources like energy since the computer has to calculate larger datasets that are often very sparse. So we opted to use many of the natural language processing libraries we had been taught in class to separate the text by part of speech and then to give the model only the pronouns, adjectives, and adverbs.
            </p>
            <h3>Model Accuracies</h3>
            <p> 
            With Support Vector Machine, we had about 95-97% accuracy. <br>
            When using K-Nearest Neighbours, our accuracy was 85-93%.<br>
            While using Linear regression, we had 92-96% accuracy.
            </p>
            <h3>View Our Code!</h3>
            <script src="https://gist.github.com/ybidochko/88ab8a9b5f0540bb9c70dfec2e8f4ab2.js"></script>
        </div>
    </body> 
</html>