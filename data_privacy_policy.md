# Data Privacy & Retention Policy

## 1. Policy Statement

This document outlines the official policy for the handling of user-submitted data for the Image Emotion Detection service. Our commitment is to ensure the highest level of user privacy by minimizing data collection and retention.

This policy directly addresses requirement **NFR-1** from the product requirements document.

## 2. Guiding Principle: Data Minimization

The core principle of our data handling strategy is **data minimization**. We will only process data that is absolutely necessary to provide the service, and we will not store any user-submitted data beyond the immediate time it takes to perform the analysis.

## 3. Data Lifecycle

The lifecycle of user data is designed to be as short as possible:

1.  **Data Reception:** A user uploads an image file via the secure (HTTPS) web interface. The image is sent to our backend service layer.
2.  **In-Memory Forwarding:** Our service layer loads the image into memory, converts it to the required format, and forwards it securely over HTTPS to our internal Azure Machine Learning endpoint for analysis. The image is **not** stored on disk by our service layer.
3.  **Analysis:** The Azure ML endpoint performs the emotion detection. Per its own data handling policies, it does not retain user data.
4.  **Response Generation:** The analysis results are returned to our service layer, which then forwards them to the user.
5.  **Data Deletion:** Immediately after the response is sent to the user, our service layer's execution ends. The memory used, including the image data, is released and purged. No data is retained.

## 4. What We Do Not Store

To be explicitly clear, we **DO NOT** store, log, or retain any of the following:

*   The original image files uploaded by the user.
*   Any copies or derivatives of the images.
*   The JSON analysis results generated for the user.
*   Any personal information that could link a user to an uploaded image.

The system is intentionally designed to be **stateless**. Each transaction is independent, and no history is maintained.

## 5. Data in Transit

All data transmitted between the user's browser and our backend services is encrypted using industry-standard HTTPS/TLS protocols. This ensures that the data is secure and cannot be intercepted during the upload process.

## 6. Policy Review

This policy will be reviewed periodically to ensure it remains aligned with privacy best practices and any applicable regulations.