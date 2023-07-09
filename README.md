# credit-risk-classification

Purpose of Analysis: Train and evaluate a model based on loan risk using a dataset of historical lending activity from a peer-to-peer lending services. Output will be a model that can identify the creditworthiness of borrowers.

The results:
- Accuracy score for the resampled model is .99, indicating the model is correct at predicting outcomes 99% of the time (predicting a "healthy" vs "unhealthy" loan). Notably, this score increased from .95 to .99 after resampling.
- Precision for resampled model is 1.0 for healthy loans, and .84 for unhealthy loans. This means that 100% of the loans deemed "healthy" by the model were truly "healthy", and 84% of the loans deemed "unhealthy" by the model were actually "unhealthy" in reality.
- Recall for the resampled model is .99 for healthy and not healthy loans. This means the model is not predicting a lot of false negatives (ex. calling an unhealthy loan healthy, or vice versa)

 A summary: Recommend implementing this model due to the overall 1) high accuracy score and 2) high recall scores (for both healthy and unhealthy loans). Having a lot of false negatives (calling a loan healthy when it is unhealthy) would be risky / costly to the company, as they'd lend out $ to individuals who likely would not repay it (ever, or in a timely manner) - this model minimizes that risk. While the precision could certainly be improved (for "unhealthy loans"), there is less risk in calling something unhealthy when it is actually healthy (we would not give a loan out to these customers, and while it is lost business, it is less risky than giving loans out to folks who won't repay them).
 
