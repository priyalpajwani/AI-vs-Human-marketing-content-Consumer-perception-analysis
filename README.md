# AI vs Human marketing content Consumer perception analysis
A data driven evaluation of generative AI's role in visual marketing content creation. 

## Overview: 
This project examines whether generative AI marketing imagery can match human created imagery in shaping consumer perception. Five AI generated marketing images were paired with five human created brand images and evaluated through a blind survey measuring quality, realism, and visual appeal. The repository contains the analysis of the resulting 7,470 ratings.

## Research question: 
Marketing teams are adopting generative AI to produce visual content at scale, yet relatively few are measuring how audiences actually respond to it. This study tests the question directly: respondents rated AI and human images without being told which was which, allowing a llike for like comparison of perception and an assessment of whether viewers can distinguish between the two.

## Data: 
1. 83 respondents, 10 images, 9 rating dimensions per image — 7,470 individual ratings in total
2. 5 AI generated images created using CHATGPT and Google Nano Banana and 5 human created brand images
3. 7 point Likert scale, supplemented by paired choice questions and demographic variables (age, gender, education, AI familiarity, social media usage)
4. Collected via a Microsoft Forms survey

## Method:
1. Built in Python (pandas, numpy, matplotlib, seaborn, plotly) within Jupyter.
2. The raw Microsoft Forms export required substantial preparation: personally identifiable and metadata fields were removed, inconsistent category labels were standardised, and free text Likert responses such as 1 (strongly disagree) were parsed into numeric values. The dataset was then reshaped into long format, one row per rating so that results could be aggregated flexibly across images, dimensions, and demographic groups.
3. The analysis proceeded from descriptive statistics (overall, by dimension, and by image) to comparative analysis of AI versus human imagery across dimensions, age groups, AI familiarity levels, and the paired choice questions. A heatmap of image by dimension performance, a ranking of evaluation dimensions, and an interquartile range outlier check which confirmed a stable distribution with no significant outliers, complete the analysis.

## Findings: 
1. AI imagery performs strongly on technical execution, professional production (5.33), clarity of detail (5.30), and overall quality (5.27) but scores lowest on realism (4.43) and natural appearance (4.51). Realism is the consistent weak point.
2. The highest and lowest rated images were a mix of AI and human origin, indicating that the quality of the individual asset is a stronger determinant of perception than whether it was AI or human produced.
3. Respondents could not reliably distinguish AI from human images. Human images were rated marginally more realistic, but identification accuracy sat close to chance.
4. Respondents with greater AI familiarity rated the two image types more similarly, suggesting the perception gap narrows as exposure to AI content increases.

In summary, AI imagery is well suited to clean, product led content, while human imagery retains an advantage in realism and people led contexts.

## Why this matters for media and entertainment platforms: 
This study measures static, AI generated imagery, which is in many respects the inverse of live, real time content, and that contrast is what makes its findings relevant to a platform built around the latter. The central result is that generative AI has largely closed the gap on polish and technical execution but not on realism and authenticity, with human content retaining its clearest advantage precisely where an image needs to feel genuine. Live content represents the strongest form of that advantage, being unscripted, unedited, and verifiably human in a way synthetic media cannot replicate. This carries a direct implication for content strategy. As feeds fill with AI generated material that viewers cannot reliably distinguish from the real thing, authenticity ceases to be a baseline that every piece of content possesses and instead becomes a scarce and therefore more valuable quality. Because the dimensions on which AI underperforms in this study are the same ones that define a live format, the proliferation of synthetic content can reasonably be read as a tailwind for real-time content rather than a threat to it, and the case for positioning live features as the authentic alternative is one these findings support rather than merely assert. Two further results bear on how such a strategy would be executed. The first is that perception was not uniform across the sample but varied with both age and familiarity with AI, which implies that any effort to drive awareness or adoption of a feature among creators and audiences should be segmented along those lines rather than delivered as a single undifferentiated message. The second is that perceived performance tracked the quality of the individual asset far more closely than its category of origin, which makes the case for evaluating content and features through measured metrics and user feedback rather than assumptions about what ought to perform well, reflecting the same test-and-learn discipline on which sound product and go to market decisions rely.

## Limitations: 

1. The survey did not ask respondents to classify each image as AI or human generated, thus the detection ability was estimated indirectly from realism ratings, a defensible proxy, but not a direct measure. A future iteration would include an explicit classification question.
2. The sample skews toward respondents aged 18–24 with existing AI familiarity: findings generalise most reliably to younger, digitally native audiences and likely overstate AI acceptance among older segments.
3. The raw survey export contained mixed text and numeric responses, irregular spacing, and inconsistent demographic labels; data cleaning accounted for a significant share of the work.

## Note: 
This project originated as a Retail and Marketing Analytics coursework assignment at Imperial College London. The survey distribution, data preparation, and Python analysis presented here are my own work.
