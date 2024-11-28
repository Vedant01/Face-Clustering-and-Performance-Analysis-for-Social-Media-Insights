# Face Clustering and Performance Analysis for Social Media Insights

## Purpose

This project was developed as part of an internship application for **FuelGrowth**, a company focused on understanding social media content and providing insights to boost performance. The goal is to analyze influencer content from videos and identify which influencer performed the best based on their appearance and associated performance scores.

### Key Objectives:

1. **Identify Influencers**: The code processes a set of social media videos to identify and group similar faces, allowing for the identification of individual influencers across multiple videos.

2. **Cluster Similar Faces**: Once faces are detected in the videos, the code uses clustering techniques to group similar faces together. This helps determine which influencers appear multiple times, even if they are featured in different videos.

3. **Performance Scoring**: Each video is associated with a performance score, representing how well the influencer performed. By grouping the faces into clusters, the code calculates the average performance score for each cluster, revealing which influencers are performing the best across all the videos.

4. **Improve Content Strategy**: By identifying high-performing influencers, the insights gained can help FuelGrowth understand which influencers are driving the most engagement and potentially suggest strategies to boost the visibility and performance of social media content.

### Two Approaches to Solve the Problem:

The project adopted **two approaches** for face clustering and performance analysis:

- **First Approach**: This method was effective but **too slow and error-prone** for large datasets. It provided accurate results but was not scalable for real-time or large-scale applications.

- **Second Approach**: After evaluating the performance of the first approach, a faster and more robust method was adopted. This second approach significantly improved the speed and accuracy of the process, making it ideal for handling larger datasets and ensuring better scalability for real-time performance tracking.

## Dataset Format

The dataset used for this analysis consists of a CSV file that contains information about each video, including the video URL and the associated performance score. The CSV file should have the following format:

|Performance Score | Video URL                                      | 
|------------------|------------------------------------------------|
| 0.85             | https://example.com/video1.mp4                 |
| 0.95             | https://example.com/video2.mp4                 |
| 1.10             | https://example.com/video3.mp4                 |
| ...              | ...                                            |

- **Video URL**: The URL of the social media video that contains the influencer’s content.
- **Performance Score**: A numerical score representing the performance of the influencer in the video, which could be based on engagement metrics such as likes, comments, views, or other relevant KPIs.

### How to Use the Dataset:
1. Place the CSV file in the project directory (update the path in the code accordingly).
2. Ensure the video URLs are valid and point to publicly accessible video files.
3. Run the code, and it will download the videos, extract frames, detect faces, compute embeddings, cluster the faces, and calculate the average performance score for each cluster of influencers.


