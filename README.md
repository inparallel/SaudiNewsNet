# Saudi Newspapers Corpus (SaudiNewsNet)
This repo contains a set of **31,030** Arabic newspaper articles alongwith metadata, extracted from various online Saudi newspapers.

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
    | aawsat | [Al-Sharq Al-Awsat](http://aawsat.com/) |
    | aleqtisadiya | [Al-Eqtisadiya](http://aleqt.com/) |
    | aljazirah | [Al-Jazirah](http://al-jazirah.com/) |
    | almadina | [Al-Madina](http://www.al-madina.com/) |
    | alriyadh | [Al-Riyadh](http://www.alriyadh.com/) |
    | alwatan | [Al-Watan](http://alwatan.com.sa/) |
    | alweeam | [Al-Weeam](http://alweeam.com.sa/) |
    | alyaum | [Al-Yaum](http://alyaum.com/)  |
    | arreyadi | [Arreyadi](http://www.arreyadi.com.sa/) |
    | arreyadiyah | [Arreyadi](http://www.arreyadiyah.com/) |
    | okaz | [Okaz](http://www.okaz.com.sa/) |
    | sabq | [Sabq](http://sabq.org/) |
    | was | [Saudi Press Agency](http://www.spa.gov.sa/) |
    | 3alyoum | [Ain Alyoum](http://3alyoum.com/) |

 - **`url`**: The full URL from which the article was extracted.
 - **`date_extracted`**: The timestamp of the date on which the article was extracted. It has the format `YYYY-MM-DD hh:mm:ss`. Notice that this field does not necessarily represent the date on which the article was authored (or made available online), however for articles stamped with a date of extraction after August 1, 2015, this field most probably represents the date of authoring.
 - **`title`**: The title of the article. Can be empty.
 - **`author`**: The author of the article. Can be empty.
 - **`content`**: The content of the article.

Statistics
----------
The dataset currently contains **31,030** Arabic articles (with a total number of **8,758,976 words**). The articles were extracted from the following Saudi newspapers (sorted by number of articles):

 - [Al-Riyadh](http://www.alriyadh.com/) (4,852 articles)
 - [Al-Jazirah](http://al-jazirah.com/) (3,690 articles)
 - [Al-Yaum](http://alyaum.com/) (3,065 articles)
 - [Al-Eqtisadiya](http://aleqt.com/) (2,964 articles)
 - [Al-Sharq Al-Awsat](http://aawsat.com/) (2,947 articles)
 - [Okaz](http://www.okaz.com.sa/) (2,846 articles)
 - [Al-Watan](http://alwatan.com.sa/) (2,279 articles)
 - [Al-Madina](http://www.al-madina.com/) (2,252 articles)
 - [Al-Weeam](http://alweeam.com.sa/) (2,090 articles)
 - [Ain Alyoum](http://3alyoum.com/) (2,080 articles)
 - [Sabq](http://sabq.org/) (1,411 articles)
 - [Saudi Press Agency](http://www.spa.gov.sa) (369 articles)
 - [Arreyadi](http://www.arreyadi.com.sa/) (133 articles)
 - [Arreyadiyah](http://www.arreyadiyah.com/) (52 articles)

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

Contacting the Maintainer
-------------------------
If you'd like to cite this work; have comments or thoughts to share; or just feel like chatting then feel free to contact me on either:

 - [My Twitter account @UniqueLock](https://twitter.com/uniquelock)
 - mazen [dot] abdulaziz [at] gmail [dot] com

Changelog
---------
 - Aug 06, 2015: 
   - First batch of articles uploaded (extracted within the period 21/07/2015 to 06/08/2015).
 - Aug 07, 2015:
   - Changed output format.
   - Included a second batch (extracted in 07/08/2015).
 - Aug 11, 2015:
   - Tracking 2 more newspapers: Saudi Press Agency and Arriyadiyah.
   - Third batch of articles updloaded (timespan: 08/08/2015 to 11/08/2015).

# License
![Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)

This work is licensed under a **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License**. The dataset is shared for the sole purpose of aiding open scientific research (in Arabic computing or linguistics), and can only be used for that purpose. The ownership of each article within the dataset belongs to the respective newspaper from which it was extracted; and the maintainer of the repository does not claim ownership of any of the content within it. If you think, by any means, that this dataset breaches any established copyrights; please contact the repository maintainer.
