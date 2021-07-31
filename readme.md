# Cultural effects on German PISA 2012 scores
## by Markus Stachl
31.07.2021


## Dataset

> PISA is the OECD's Programme for International Student Assessment. PISA measures 15-year-olds’ ability to use their reading, mathematics and science knowledge and skills to meet real-life challenges. I restricted the dataset to reponses from German students.

> The main goal is to analyse how the cultural and educational backgroud of students influence their school performance indicated by the PISA test results. I also want to highlight possible struggles of immigrants in Germany.

> As schools were categorized using float values, I needed to transform them into categorical strings. Therefore I mapped float values to a describing string translating school names from the PISA 2012 scale handbook

### Features of interest:
> **Test scores:**
> - Mathematics score: PV1MATH
> - Reading score: PV1READ
> - Science score: PV1SCIE

> **Student information:**
> - Country: CNT
> - Gender of student: ST04Q01
> - National study program (type of attended school): ST02Q01

> **Family information:**
> - Education level father: FISCED
> - Education level mother: MISCED
> - Highest education level parents: HISCED
> - Family structure: FAMSTRUC
> - Immigration status: IMMIG


## Summary of Findings

> **Test scores**: 
> - All scores - `math_score`, `reading_score` and `science_score` -  are approximately normal distributed and centered arount 500. Most students score between 300 and 750 on each test. On average, students tend to perform slightly better (arount 20 points) on the `science_score` compared to reading and mathmatics.
> - Germany performed above OECD average in all three test subjects.
> - On the mathematics test, male students performed slightly better on average, by 20 points. On the contrary, females scored better on the reading test, also by 20 points. When it comes to science, female and male students in Germany performed equally well on the PISA 2012 test.

> **School types**:
> - Attended school is a gread indicator for attained scores for each student. This is possibly due to the different level of education in general and therefore expected.
> **Family structure and education**: 
> - Availability of both parents does not have an influence on students school performances. Students raised by a single parent (father or mother) perform equally well in all three test subjects. This is counter-intuitive, since I expected kids' performances to depend on support given by their parents and single parents tend to have less time for their kids as they have to juggle several responsibilities on their own.
> - Nevetheless, students living in other familily structures (no parents, living with grandparents etc.) tend to perform significally lower compared to the othe two categories. Finding reasons for this could be open for further research.
> 
> **Immigration status**:
> - Native students scored on average 550 on all three tests. First and second-generation immigrations performed lower (by about 10%). From the boxplots above, I derive that immigrants in general struggle more in school and perform less compared to native students. Second-generation immigrants perform better than first-generation immigrants, giving rise to the assumption that this effect is weakened with the timing spend in the migrated country.

## Sources
- PISA 2012 survey: https://www.oecd.org/pisa/data/
- PISA 2012 codebook: https://www.oecd.org/pisa/pisaproducts/PISA12_stu_codebook.pdf
- PISA 2012 scale book (German): https://www.pisa.tum.de/fileadmin/w00bgi/www/Berichtsbaende_und_Zusammenfassungungen/PISA_2012_Skalenhandbuch_final-openaccess.pdf
