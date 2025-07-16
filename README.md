# Face Blur AI – Real-Time Face Anonymization API

Face Blur AI is a high-performance, deep learning–powered API that detects and blurs human faces in any image. Built for speed, accuracy, and privacy, it supports multi-face detection, customizable blur strength, and returns results in under 1 second.

Ideal for developers building tools for content moderation, privacy compliance (e.g., GDPR, CCPA), or anonymization of public or sensitive data.

---
<p float="left">
<img width="500" height="360" alt="blur_face_15487215" src="https://github.com/user-attachments/assets/f0d0145e-4215-49a8-ab62-a415a9cfea4e" /> 
<img width="500" height="360" alt="blur_face_14527844" src="https://github.com/user-attachments/assets/b4ed9475-6b65-4fa9-9f84-c002e96cda82" />
</p>


## Features

-  **Accurate AI Face Detection**  
  Detects multiple faces per image, including front-facing, side views, and partial faces.

-  **Adjustable Blur Strength**  
  Control how strong the blur effect is via the `blur_strength` parameter (1–10).

-  **Real-Time Performance**  
  Sub-second image processing makes it ideal for high-volume use cases.

- **Privacy-First Architecture**  
  No images are stored. All processing happens in-memory, ensuring full GDPR compliance.

- **Easy Integration**  
  Simple HTTP POST request — no training, setup, or ML expertise required.

-  **Supports JPG and PNG**  
  Accepts standard image formats and returns the blurred image.

---

 **The example image  to compare the blur effect at different levels (1–10):**
 
<img width="1000" height="400" alt="blur_face_485144788" src="https://github.com/user-attachments/assets/da374e24-3473-4655-b5da-2963941b30c6" />

---



## API Overview

The Face Blur AI API uses state-of-the-art deep learning models to:
- Automatically detect all human faces in a provided image
- Apply high-quality, pixel-level Gaussian blur to each detected face
- Return a processed image while maintaining the original dimensions

It works seamlessly on:
- Solo portraits
- Group photos
- Crowds
- Partially visible or turned faces


**Code Snippets**
```shell
curl --request POST 
	--url https://face-blur-ai.p.rapidapi.com/api/v1/blur_face 
	--header 'Content-Type: multipart/form-data' 
	--header 'x-rapidapi-host: face-blur-ai.p.rapidapi.com' 
	--header 'x-rapidapi-key: YOUR_RAPIDAPI_KEY' 
	--form image=image.jpg 
	--form blur_strength=10
```
---

## Get Started

You can try the API directly here:

👉 RapidAPI – [Venify Face Blur AI](https://rapidapi.com/venify-venify-default/api/face-blur-ai)


### Postman Collection
This Postman collection includes ready-to-use requests for blurring faces:

 #### How to Use

1. Download [the collection JSON](./Venify_Face_Blur_API.postman_collection.json) or clone this repo
2. Open Postman and click “Import”.
3. Select the file: **Venify_Face_Blur_API.postman_collection.json**
4. Add your RapidAPI key in the headers or use an environment variable.
5. Start sending requests and previewing image responses.

---

## Use Cases
- Moderate user-generated content
- Anonymize surveillance or research images
- Create public datasets without exposing identities
- Protect children’s faces in photos
- Censor content in journalism or public reports
  
---

## License
This API is provided by [Venify on RapidAPI](https://rapidapi.com/venify-venify-default/api/face-blur-ai). Please refer to their usage terms, pricing, and limits.

