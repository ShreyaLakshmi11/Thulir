# THULIR - Smart Crop Health and Yield Advisory System

THULIR is a team project designed to help farmers understand crop health and make informed farming decisions through a mobile application.

The project brings together leaf-image analysis, crop-care guidance, yield prediction, crop recommendations and market-price forecasting. English, Hindi and Tamil support, along with read-aloud audio, are included in the application design to make information easier to access.

## Project goals

- Identify potential crop diseases from leaf images
- Present crop-care and prevention guidance in simple language
- Provide yield-related guidance and suitable crop recommendations
- Forecast crop market prices
- Combine findings into a report with local-language and audio support

## Designed workflow

1. The farmer selects a language and captures or uploads a leaf image.
2. The image is checked and processed for crop-health analysis.
3. Disease findings are combined with yield guidance, crop recommendations and price forecasts.
4. An AI explanation layer presents the information in simple language.
5. The farmer views the report and can use the read-aloud option.

## Model choices by task

| Task | Model in the project design |
| --- | --- |
| Image classification | Vision Transformer (ViT) with TabNet |
| Disease prediction | MobileNet |
| Yield prediction | TabNet |
| Market-price forecasting | Prophet |

The crop-recommendation module considers soil nutrients (nitrogen, phosphorus and potassium), temperature, humidity, pH and rainfall. A specific recommendation algorithm is not documented here.

## Technology design

- Flutter and Dart for the mobile application
- Python and Flask for the backend
- OpenCV for image processing
- Generative AI for simple-language explanations
- Text-to-speech for audio support

## Screenshots

App screenshots are presented below to illustrate the interface and report design.

<img width="720" height="1502" alt="WhatsApp Image 2026-11-12 at 2 12 01 PM" src="https://github.com/user-attachments/assets/3d29eda2-3ae9-44d6-9364-36a112f80fad" />
<img width="720" height="1505" alt="WhatsApp Image 2026-11-12 at 2 12 10 PM" src="https://github.com/user-attachments/assets/f14bccf8-e926-4bad-9a54-9a41cca66284" />
<img width="720" height="1503" alt="WhatsApp Image 2026-11-12 at 2 12 16 PM" src="https://github.com/user-attachments/assets/e8d8c711-23f6-4dbc-8b53-88b2845c212b" />
<img width="720" height="1503" alt="WhatsApp Image 2026-11-12 at 2 12 23 PM" src="https://github.com/user-attachments/assets/8af04846-3d85-453a-b643-9a07dd27d4a0" />

## About this repository

This repository is a showcase of the THULIR team project and its application screens. It is not currently presented as a complete, reproducible source-code release.

The model descriptions explain the project architecture. Screenshots alone do not establish live model integration, prediction accuracy or real-time market data. No independently verified performance metrics are claimed here.

## Limitations

THULIR is a crop-health and farming advisory application. Its predictions and generated advice may be incomplete or incorrect. Crop treatment decisions should be checked with a qualified agricultural professional, and market forecasts should not be treated as guaranteed prices or returns.
