### Project Overview:
Conducted advanced text classification using transfer learning with HuggingFace's Transformer model to categorize over 2,000 Facebook posts into three distinct categories.

### Background:
In the vast landscape of social media, Facebook stands out as a prominent platform for businesses to engage with their audience. Business pages on Facebook receive a constant stream of user-generated content, including posts that convey customer feedback, complaints, and appreciations. Analyzing this wealth of data presents a unique opportunity for businesses to gain real-time insights into customer needs and preferences.

### Dataset and Task:
Utilized a labeled dataset named "FB_posts_labeled.txt" with the following key fields:

#### postId: Unique identifier for each user post (7961 posts in total).

#### message: Textual content of each post.

#### Appreciation: Binary indicator (0/1) for posts expressing appreciation.

#### Complaint: Binary indicator (0/1) for posts containing customer complaints.

#### Feedback: Binary indicator (0/1) for posts categorized as customer feedback (questions and suggestions).

These three classes—Appreciation, Complaint, and Feedback—constitute the content categories in the dataset. Though human-labeled, acknowledging the potential for labeling nuances, we treat these annotations as ground truth for the task. The objective is to construct a text classifier capable of predicting the content category of a post based on its textual content.

### Evaluation and Unlabeled Dataset:
To assess the model's out-of-sample performance, predictions are generated for 2039 posts in an unlabeled dataset named "FB_posts_unlabeled.txt." This dataset includes postId and message fields. The ground truth labels for these posts are kept confidential, ensuring an impartial evaluation. The performance metric employed is the averaged F-measure across the three content categories.

### This project addresses the nuanced task of classifying diverse Facebook posts, providing businesses with a powerful tool to understand and respond to customer sentiments effectively.
