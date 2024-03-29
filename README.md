Kenny Burrell & Donald Byrd1.
Biography...
One of the leading exponents of straight-ahead jazz guitar, Kenny Burrell is a highly influential artist whose understated and melodic style, grounded in bebop and blues, made him in an in-demand sideman from the mid-’50s onward and a standard by which many jazz guitarists gauge themselves to this day. Born in Detroit in 1931, Burrell grew up in a musical family in which his mother played piano and sang in the Second Baptist Church choir, while his father favored the banjo and ukulele. Burrell began playing guitar at age 12 and quickly fell under the influence of such artists as Charlie Christian , Django Reinhardt , Oscar Moore, T-Bone Walker , and Muddy Waters . Surrounded by the vibrant jazz and blues scene of Detroit, Burrell began to play gigs around town and counted among his friends and bandmates pianist Tommy Flanagan , saxophonists Pepper Adams and Yusef Lateef , drummer Elvin Jones , and others. In 1951, Burrell made his recording debut on a combo session that featured trumpeter Dizzy Gillespie as well as saxophonist John Coltrane , vibraphonist Milt Jackson , and bassist Percy Heath. Although his talent ranked among the best of the professional jazz players at the time, Burrell continued to study privately with renowned classical guitarist Joe Fava, and enrolled in the music program at Wayne State University. Upon graduating in 1955 with a B.A. in music composition and theory, Burrell was hired for a six-month stint touring with pianist Oscar Peterson ’s trio. Then, in 1956, Burrell and Flanagan moved to New York City and immediately became two of the most sought-after sidemen in town, performing in gigs with such luminaries as singers Tony Bennett and Lena Horne , playing in Broadway pit orchestras, and recording with an array of legendary musicians including Coltrane , trumpeter Kenny Dorham , organist Jimmy Smith , vocalist Billie Holiday , and many others. Burrell made his recorded debut as a leader on the 1956 Blue Note session Introducing Kenny Burrell — technically his second session for the label, but the first to see release. From the late ’50s onward, Burrell continued to record by himself and with others, and has appeared on countless albums over the years including such notable albums as 1957′s The Cats featuring Coltrane , 1963′s Midnight Blue featuring saxophonist Stanley Turrentine , 1965′s Guitar Forms with arrangements by Gil Evans , and 1968′s Blues -- The Common Ground . Beginning in 1971, Burrell started leading various college seminars including the first regular course to be held in the United States on the music of composer, pianist, and bandleader Duke Ellington . He continued performing, recording, and teaching throughout the ’80s and ’90s, releasing several albums including 1989’s Guiding Spirit, 1991′s Sunup to Sundown, 1994′s Collaboration with pianist LaMont Johnson , 1995′s Primal Blue, and 1998′s church music-inspired Love Is the Answer. In 2001, Burrell released the relaxed quartet date A Lucky So and So on Concord and followed it up in 2003 with Blue Muse. He celebrated turning 75 years old in 2006 by recording a live date, released a year later as 75th Birthday Bash Live! In 2010, Burrell released the live album Be Yourself: Live at Dizzy's Club Coca-Cola, recorded at Lincoln Center’s smaller club-like venue, followed two years later by Special Requests (And Other Favorites): Live at Catalina's. In 2015, Burrell released The Road to Love, recorded live at Catalina’s Jazz Club in Hollywood. Another Catalina’s live date, Unlimited 1, appeared in 2016 and featured Burrell backed by the Los Angeles Jazz Orchestra. Besides continuing to perform, Burrell is the founder and director of the Jazz Studies Program at UCLA, as well as president emeritus of the Jazz Heritage Foundation. ~ Matt Collar & Al Campbell..



# Word.
#Simple abundanceMethodist for enlightenment.
# 20221031-PY
2022-10-31 
This problem was asked by Google.
You are given a set of synonyms, such as (big, large) and (eat, consume). Using this set, determine if two sentences with the same number of words are equivalent.

For example, the following two sentences are equivalent:

"He wants to eat food."
"He wants to consume food."
Note that the synonyms (a, b) and (a, c) do not necessarily imply (b, c): consider the case of (coach, bus) and (coach, teacher).

Follow-up: what if we can assume that (a, b) and (a, c) do in fact imply (b, c)?

Solution
For the first problem, we must create a data structure that allows us to simply check whether any two words are synonyms. We can achieve this by making a dictionary whose keys are all the distinct words in our set, and whose values are their synonyms.

Once we have this data structure, we will split each sentence into words and iterate over each pair. If for every pair, either the words are identical, or one word can be found as a value corresponding to the other's key, then the two sentences are equivalent.
