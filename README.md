![AutoBLUR Logo](https://github.com/philip-hawkins-git/AutoBLUR/blob/main/AutoBLUR_Banner.png)

# AutoBLUR: Automated Brand Obfuscation Tool
AutoBLUR is an advanced tool designed to automate the process of removing identifiable brand elements from video content. It is particularly useful for market research and memorability testing, where unbiased recall of brand information is crucial.

## Key Features:
1. Automated Video Processing:

* Downloads and extracts video files from a specified URL.
* Processes videos by blurring brand logos and text using computer vision techniques.
  
2. Dual Engine Capability:

* EasyOCR: Detects and blurs text within video frames.
* YOLO (You Only Look Once): Identifies and blurs brand logos with high accuracy.
  
3. Customizable Confidence Level:

* Users can adjust the confidence threshold to control the sensitivity of text and logo detection.
  
4. Efficient Workflow:

* Processes each video frame-by-frame, applying blurring to detected regions.
* Outputs processed videos to a designated directory, ensuring easy access and organization.
  
5. Robust Error Handling:

* Includes mechanisms to handle errors during video processing, ensuring smooth operation.
  
6. Model Integration:

* Utilizes a pre-trained YOLO model to enhance logo detection accuracy.
* Automatically downloads the model if not present, simplifying setup.
  
## Usage:
AutoBLUR is ideal for researchers and analysts who need to strip branding from videos for unbiased testing. It automates the labor-intensive task of manual editing, enhancing efficiency and accuracy in market research scenarios.

The model was trained to recognize the following brand logos:

* Auto: Acura, Audi, Chevy, Ford, Ford Mustang, Honda, Hyundai, Infiniti, Lexus, Nissan, Subaru, Toyota, Volkswagen
* Clothing: Adidas
* Delivery: Shipt
* Entertainment: NBC, Paramount, Univision
* Finance: American Express, Capital One, Chase, H&R Block, TurboTax Food/Drink: MuscleMilk
* Gambling: BetMGM, DraftKings, FanDuel
* Home: Behr, Benjamin Moore, Lowe's
* Insurance: Farmers, Liberty Mutual, State Farm
* Pharmaceuticals: Pfizer, Prevnar, Dupixent
* Restaurant: Burger King, Chick-fil-A, Domino's, KFC, Pizza Hut, Subway, Wendy's
* Retail: Amazon, Macy's, Target, Walmart
* Telecom/Technology: Apple, AT&T, Boost, Spectrum, T-Mobile, US Cellular, Verizon, Xfinity
* Travel: Delta, Expedia

## Instructions
AutoBLUR is designed for ease of use:

1. Specify Video Location:

* Indicate where your MP4 files are stored. Test examples are available at /content/Videos/UnblurredVideos/.

2. Adjust Confidence Level:
   
* Set the confidence level slider. A higher value reduces false positives.
  
3. Run the Tool:
  
* Click the run button to start processing.
  
The processed videos will be saved in the content/AutoBlurVideos/ folder, accessible on the left side of the notebook.

Note: For optimal performance, use a GPU. You can enable this by selecting "Runtime" > "Change runtime type" and choosing "T4 GPU".
