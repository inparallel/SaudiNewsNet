# Saudi Newspapers Corpus (SaudiNewsNet)
This repo contains a set of 24,669 Arabic newspaper articles alongwith metadata, extracted from various online Saudi newspapers.

File Structure
--------------
The folder `dataset` contains a set of ZIP files, where each file has the format `YYYY-MM-DD.zip` and contains one JSON file with a corresponding name `YYYY-MM-DD.json`. The JSON files are stored in UTF-8 encoding.

Each JSON file contains an array of articles (the format of each article is explained in the next section), and its file name reflects the date on which the contained articles were extracted.

Article JSON Object Format
--------------------------
The JSON object for each article contains the following fields (some fileds can have empty values in case the crawler failed to extract them):

 - **`source`**: A string identifief of the newspaper from which the article was extracted. It can have one of the following values:

    | String Identifier  | Newspaper |
    | ------------------ | --------- |
    | aawsat | [Al-Sharq Al-Awsat](aawsat.com/) |
    | aleqtisadiya | [Al-Eqtisadiya](http://aleqt.com/) |
    | aljazirah | [Al-Jazirah](http://al-jazirah.com/) |
    | almadina | [Al-Madina](http://www.al-madina.com/) |
    | alriyadh | [Al-Riyadh](http://www.alriyadh.com/) |
    | alwatan | [Al-Watan](http://alwatan.com.sa/) |
    | alweeam | [Al-Weeam](http://alweeam.com.sa/) |
    | alyaum | [Al-Yaum](http://alyaum.com/)  |
    | arreyadi | [Arreyadi](http://www.arreyadi.com.sa/) |
    | okaz | [Okaz](http://www.okaz.com.sa/) |
    | sabq | [Sabq](http://sabq.org/) |
    | 3alyoum | [Ain Alyoum](http://3alyoum.com/) |

 - **`url`**: The full URL from which the article was extracted.
 - **`date_extracted`**: The timestamp of the date on which the article was extracted. It has the format `YYYY-MM-DD hh:mm:ss`. Notice that this field does not necessarily represent the date on which the article was authored (or made available online), however for articles stamped with a date of extraction after August 1, 2015, this field most probably represents the date of authoring.
 - **`title`**: The title of the article. Can be empty.
 - **`author`**: The author of the article. Can be empty.
 - **`content`**: The content of the article.

Statistics
----------
The dataset currently contains 24,669 Arabic articles (with a total number of **7,060,353 words**). The articles were extracted from the following Saudi newspapers (sorted by number of articles):

 - [Al-Riyadh](http://www.alriyadh.com/) (3,855 articles)
 - [Al-Jazirah](http://al-jazirah.com/) (2,892 articles)
 - [Al-Sharq Al-Awsat](aawsat.com/) (2,466 articles)
 - [Al-Yaum](http://alyaum.com/) (2,405 articles)
 - [Al-Eqtisadiya](http://aleqt.com/) (2,352 articles)
 - [Okaz](http://www.okaz.com.sa/) (2,250 articles)
 - [Al-Watan](http://alwatan.com.sa/) (1,800 articles)
 - [Al-Weeam](http://alweeam.com.sa/) (1,736 articles)
 - [Ain Alyoum](http://3alyoum.com/) (1,715 articles)
 - [Al-Madina](http://www.al-madina.com/) (1,676 articles)
 - [Sabq](http://sabq.org/) (1,392 articles)
 - [Arreyadi](http://www.arreyadi.com.sa/) (130 articles)

Citing this Work
------------------

If you'd like to cite this work, you may use one of the following. You may also contact me (mazen [dot] abdulaziz [at] gmail [dot] com) so that I can include your research in the "referring work" section.

 - **APA**: Alhagri, M. A. (2015). Saudi Newspapers Arabic Corpus (SaudiNewsNet). http://github.com/ParallelMazen/SaudiNewsNet
 - **MLA**: Alhagri, Mazen A. Saudi Newspapers Arabic Corpus (SaudiNewsNet). 2015. http://github.com/ParallelMazen/SaudiNewsNet
 - **BibTex**: 
  `@misc{hagrima2015,
  author = "M. Alhagri",
  title = "Saudi Newspapers Arabic Corpus (SaudiNewsNet)",
  year = 2015,
  url = "http://github.com/ParallelMazen/SaudiNewsNet"
  }`

Changelog
---------

 - Aug 06, 2015: First batch of articles uploaded (extracted within the period 21/07/2015 to 06/08/2015).
 - Aug 07, 2015: Changed output format. Included a second batch (extracted in 07/08/2015).

# License
![Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)

This work is licensed under a **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License**. The dataset is shared for the sole purpose of aiding open research in Arabic computing. The ownership of each article within the dataset belongs to the respective newspaper from which it was extracted; and the maintainer of the repository does not claim ownership of any of the content within it. If you think, by any means, that this dataset breaches any established copyrights; please contact the repository maintainer.




