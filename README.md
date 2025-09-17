#Automated Detection of Fraudulent Rental Posts on Facebook: Combining LLM with Open Source Intelligence

##Abstract
The growth of rental scams on social media, especially on Facebook, is becoming increasingly pervasive, which is particularly true among students searching for low-cost accommodation. Padova
is a very competitive market for rent because of the University of Padova and its large population
of Erasmus, local, and international students. Scammers target Facebook groups by posting fraudulent rental advertisements and comments under rent posts with unrealistically low prices, unclear
details, or requests for private communication. They are often targeting some users who often
overlook warning signs due to urgent housing needs. Existing detection methods are primarily
focused on platforms like Craigslist, which have failed to address the real-time and communitybased dynamics of Facebook public groups, leaving a critical gap in proactive scam identification.
This thesis proposes a dual method for identifying the fraudulent rental listings using prompt
engineering-based Large Language Models (LLMs) and Open Source Intelligence (OSINT) techniques. Using the OSINT tool Apify, we collected 2,189 rental posts from the public Facebook group
"AFFITTI PADOVA: STUDENTI/LAVORATORI CHE VIVONO/VORREBBERO VIVERE A
PADOVA." The dataset contained links, user IDs, advertisement contents, prices, images, addresses, and interactions (likes, comments, shares). The dataset was manually checked and labeled
into categories: "Legitimate," "Suspicious," "Uncertain," and "Fake." Such classification was based
on features such as price, images, address, user activity, interactions, and communications. We
identified 32 fake posts through manual verification and generated 75 synthetic fake posts using
a template-based method. This method analyzes suspicious and fake posts from the dataset and
creates synthetic posts that are nearly identical to the original fake posts by maintaining the structure, incorporating vocabulary patterns, and adding statistically learned suspicious patterns, such
as the lack of price, images, or detailed information. Two detection methods were developed and
evaluated. One approach is a prompt engineering-based Large Language Model approach with
the higher True Positive Rate of 0.969 on the original manually checked datasets and 0.935 after
augmentation and the lower False Positive Rate of 0.254 on the original manually checked datasets
and 0.254 after augmentation. The other approach is a Random Forest (RF) model with the lower
True Positive Rate of 0.719 on the original manually checked datasets and 0.449 after augmentation and the higher False Positive Rate of 0.372 on the original manually checked datasets and
0.405 after augmentation. This shows that the prompt engineering-based Large Language Model
outperformed the Random Forest model. Observations of unusual user behavior, including some
suspicious activities, provided key insights into potential scam indicators. Examples include multiple comments offering rooms on several "Looking for rent" posts and the posting of many rental
posts without prices or images. These examples were the primary reasons for suspicious activity.
Scammers in particular posted advertisements and got banned and deleted from the group alongside their posts. They also targeted the comments section of the renters’ posts to reach prospective
victims through private emails or Messenger accounts, where they could bypass the platform’s security measures. Engaging directly with suspected advertisers and commenters allowed us to expose
prevalent deceptive practices, such as requesting payment of half a deposit using PayPal. This
work highlights and tries to fill an important gap in real-time scam detection through manual post
verification, which is enhanced by direct chatting with the suspicious advertisers and commenters.
