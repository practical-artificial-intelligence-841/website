---
title: Bias in Machine Learning
weight: 1
---

## Jackie Alcine Story 

- 2015, Google Photos image recognition feature: grouping photos with thematic caption 

- Jackie Alcine found that dozens of Alcine’s and his friend’s photos were grouped under “gorillas” 

- Twitter exchanges 

    - Alcine’s post: “My friend is not a gorilla. Google Photos y’all f[*] up” 

    - Google chief architect, Yonatan Zunger,  replies: “ This is 100% not OK” 

- Google actions 

    - Within hours, Google removed the label “gorilla” and redeployed the tool. Still problematics 

    - After 2015, gorilla” was censored from searches and image tags 

    - In 2018, Google manually deactivates the label, as a result not even gorillas could be labelled gorilla 

    - Chimp, chimpanzee, monkey, etc., also blocked 

    - In the end, purged from the image classifier algorithm 

- The algorithm was stochastic gradient descent. Reminder: 

    - Go through training at random (stochastic) and 

    - Tune model’s parameters to assign slightly higher probability to the correct category  

    - Repeat as needed 

- The core Idea of supervised learning 

    - Can learn ANYTHNIG from examples, including bias 

- Question: how did the bias get there in the first place? 

## Photography and Bias - Frederick Douglas Story 

- Abolitionist author and lecturer who escaped slavery 

- The most photographed American in the 19th century (more than Lincoln and Ulysses Grant) 

- Douglas’s Letter to Louis Prang June 14th, 1870, in response to the lithographic portrait of the first African American US senator, Hiram Revels: 

    - “Whatever may be the prejudices of those who may look upon it, they will be compelled to admit that the Mississippi senator is a man, and one who will easily pass for a man among men. We colored men so often see ourselves described and painted as monkeys, that we think it a great piece of good fortune to find an exception to this general rule.”  

- In 1923, W.E.B. Du Bois encourage young Black people to consider the photographer career since they will know more about portraying Black people 

## Kodak’s “Shirley Card” Story 
- Lack of racial diversity in film or TV has been not only **in front of the camera**, or **behind the camera**, but also **inside the camera** 

- There have been skin-tone biases within the visual reproduction technology itself 

- Chemical processing of film was tuned to a test picture  of a White woman for color-balanced benchmark, called “Shirley card” 

- Thus, cameras weren’t taking good photos of Black people, since they were calibrated to white skin 

- In 1960s and 70s Kodak creates film sensitive to darker tones not because of correcting photos of Black people, but because of the furniture and chocolate industries and their demand for better advertisement photos 

Morale: Better classifiers depend on more data (less data make worse predictions). And more data expose representation relative to the general population that the societal structures have promoted 

- Example: More men in tech, more women in child care and the nursing profession 

## Gender Shades 

- 2010, Georgia Tech, Joy Buolamwini is an undergraduate student, using an off-the-shelf face recognition library to program a robot to play peekaboo and recognize the programmer’s face 

- The culprit is not the algorithm but the dataset of images on which the off-the-shelf model was pretrained.  

- 2007, Labeled Faces in the Wild (LFW) dataset was assembled from online news at UMass Amherst (Huang et al.) 

- 2014 LWF was analyzed: 77% male, 83% White. In 2019, LWF offered a disclaimer.  

- 2015, IJB-A dataset (IARPA Janus Benchmark A) 

    - See description at https://paperswithcode.com/dataset/ijb-a: has facial images with a wide variations in pose, illumination, expression, resolution and occlusion.  

    - 5,712 images and 2,085 videos from 500 identities, with an average of 11.4 images and 4.2 videos per identity 

## Buolamwini and Gebru Work 2017 - 2018
- Analysis of IJB-A dataset 

    - Overrepresentation of light-skin images and male images: 75% male, 80% light-skinned 

    - Underrepresentation of dark-skinned females, 4.4% 

- How to build a more representative dataset? Answer: Parliament method 

    - Select 6 nations’ parliaments: 3 from Africa and 3 Scandinavian 

        - Contain roughly equal proportions of all six skin-tone categories 

    - Tested the dataset on 3 systems: Microsoft, IBM, Megvii (China) 

    - Results 

        - Classification by gender: 90% accuracy 

            - But 10%-20% more accurate for male faces than female faces 

            - And 10%-30% more accurate on lighter faces than darker faces 

        - Intersectionality analysis of gender and skin color: dramatically worse accuracy 

            - both female and dark skin: 35% error rate 

            - but 0.3% error rate for male light skin 

## Combating Bias and Activism 
- See Joy Buolamwini’s “AI, Ain’t I a Woman”, paraphrasing the abolitionist and women’s right activity Sojourner Truth.  

- One of the 1st articles on bias in computing: Batya Friedman and Helen Nissenbau, 1996 

- The ethical accuracy question: 

    - On What? 

    - For Whom? 

- Every ML system is kind of a parliament 

    - Representing the larger electorate 

    - Should ensure that everyone gets a vote 

- Question: What if the world itself is biased? 

## References 

Joy Buolamwini. 2019. AI, Ain’t I a Woman? Vision and Justice. Radcliffe Institute.  https://youtu.be/HZxV9w2o0FM  

Joy Buolamwini. 2017. How I’m fighting bias in algorithms. TED Talk. https://www.media.mit.edu/posts/how-i-m-fighting-bias-in-algorithms/  

Batya Friedman and Helen Nissenbaum. 1996. Bias in computer systems. ACM Trans. Inf. Syst. 14, 3 (July 1996), 330–347. https://doi.org/10.1145/230538.230561  

Gender Shades. 2018. MIT Media Lab. http://gendershades.org/overview.html  

YouTube. 2018. Sojourner Truth’s “Ain’t I a Woman” Performed by Kerry Washington. https://youtu.be/Ry_i8w2rdQY  


## Optional References 

Hu Han and Anil K Jain. 2014. Age, gender, and race estimation from unconstrainted face images. https://api.semanticscholar.org/CorpusID:16095861  

Michele Merler, et al. 2019. Diversity in Faces. https://arxiv.org/abs/1901.10436. See also https://exposing.ai/ibm_dif/  

Kate Crawford and Trevor Paglen, “Excavating AI: The Politics of Training Sets for Machine Learning (September 19, 2019). https://excavating.ai/  

Gebru, Timnit. 2020. Race and Gender. In Markus D. Dubber, Frank Pasquale, and Sunit Das (eds), The Oxford Handbook of Ethics of AI (online edn, Oxford Academic, 9 July 2020), https://doi.org/10.1093/oxfordhb/9780190067397.013.16, accessed 3 Aug. 2023. 