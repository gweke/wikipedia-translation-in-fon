# wikipedia-translation-in-fon
This is a project aims to translate all wikipedia artciles from french to fon (a local languague spoken in Benin Republic)

# Ressources
For the project we will use google colab and python languague, but you can use any vm thath suit you. As a translation api, we use azure open ai with our key, endpoint and version name that you need to replace with yours.

# Steps
1. To get all artcicles contents from wikipedia, we'll use their api and not othe python library. so the first step here, is extract all articles name list from wikipedia. as written this, the total number of articles in french is 2_680_047. Like you're thinking, this is huge and will take some time to get.
2. Based on that articles list, we'll then extract all their content (not including others content like discussions, category, files, comments, etc.). As the total number of articles is huge, extracting once their content using api with its limit in terms of request, is not practicall. So we will made many different and successive extraction and in batches of let's say 10,000 (ajust this as the capacity of your materials)
3. Next, we will translate all the content from french to fon. I use a azure open ai first but the result isn't apparently in fon, is like another africans languague. So we'll test free google translate or an official one in the future

# Specifications
To execute this notebook, as we run it in google colab we use some specifications : like "!" before pip and for saving files we precede it by "/content/drive/MyDrive/". So if you want to run it locally or another vm, feel free to ajust it.

#  Update
we'll keep updated this project as per future tools or knowledge such as automatically confirm or improve translation from others sources and documentations

# Others
This first version is not already finalise and we'll be adding codes. So use it with cautions.
