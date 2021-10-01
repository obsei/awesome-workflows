# Workflow

 - GoogleNews Observer search and fetch google news article with given query
 - Then TextSplitter split article in small chunks so Classification Analyzer can process it easily
 - Then Classification Analyzer classify chunks in given labels using [HuggingFace zero shot models](https://huggingface.co/models?pipeline_tag=zero-shot-classification)
 - Then Inference Aggregator aggregate classification output for each chunks and compute final inference based on given aggregation function
 - And finally Slack Informer send result to given slack channel using API
 
![image](https://user-images.githubusercontent.com/19303690/130244375-693e0ea2-7d71-4a07-87da-e8dc3332885f.png)

Screenshot of final result -
- Full article text
![image](https://user-images.githubusercontent.com/19303690/130246209-91490dfa-3350-4a1e-a502-97e05000d937.png)
- Final article classification result
![image](https://user-images.githubusercontent.com/19303690/130246280-e6941719-abda-42e2-a993-a26e08cc38ef.png)

This [link](https://github.com/obsei/obsei#how-to-use) might help you to regarding how collect credetials of observers (Facebook, Twitter etc) and informers (Slack, Zendesk etc).
