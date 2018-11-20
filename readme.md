# Migrate PDF Content

[Tags Rob Didn't Create](https://github.com/dabobert/iab_conversion/wiki/Tags-Rob-Didn't-Create)

[Video](https://bluejeans.com/s/h93V4)

[Login Page](https://iabstaging.wpengine.com/wp-login.php?itsec-hb-token=iabadmin)


[Original page](https://iab.com/insights/themobileidguide/)

[Original PDF](https://www.iab.com/wp-content/uploads/2017/06/Mobile-Identity-Guide-for-Marketers-Report.pdf)

[Rob's sample migration](https://iabstaging.wpengine.com/insights/themobileidguide/)

## Select an article to convert

Go to [https://goo.gl/c2yQRF](https://goo.gl/c2yQRF) and assign a document to yourself

IAB articles are top priority 

## Login into WP Admin


[Login](https://iabstaging.wpengine.com/wp-login.php?itsec-hb-token=iabadmin) into the WPAdmin area


## Create a new `Insight` for the content
Create a new [insight](https://iabstaging.wpengine.com/wp-admin/post-new.php?post_type=iab_insight)

Copy and paste text from pdf file into inline wordpress content

### Link to the original PDF document

At the top of the page have a link to the original pdf with the class `pdf_download_link

```<a href="xxx" class=" pdf_download_link">Download</a>```

### Make sure the topics/tags, author and the post_date match the source
The topics/tags, `author` of the new `insight` and the `post_date` of the new insight
**MUST** match that of the original source document

ALSO COPY OVER LARGE IMAGE


### No need for paragraph tags

When editing content in HTML/Source code mode, there is no need for paragraph tags `<p>`. They are put around content with line breaks

For example:

```
This is content

This is also content
```

Gets automatically converted to 

```
<p>
This is content.
</p>

<p>
This is also content.
</p>
```

### Creating Table of contents

A table of contents must be created for the document.

Use `<h3 class="toc">Title</h3>` for main headings.

Use `<h4 class="toc">Sub-Title</h4>` for sub-headings.



### Insert Images

Use [https://www.pdfaid.com/ExtractImages.aspx](https://www.pdfaid.com/ExtractImages.aspx) to extract images form pdfs.  Sometimes no images will be found, in that case use cropped screenshots

[Taking Snippets on PC](https://support.microsoft.com/en-us/help/13776/windows-use-snipping-tool-to-capture-screenshots)

[Taking Snippets on Mac](https://www.cnet.com/how-to/three-ways-to-take-a-screenshot-on-a-mac/) TLDR; Command+Shift+4

When uploading images make sure the large size is selected

## Hero Image 

<img src="bla.jpg" id="iab-hero-image">

## Add Meta Data 

1. Wordpress 
2. "Yoast SEO" field 
3. Snippet Review 
4. Edit Snippet 
5. Add first paragraph of article to Meta Description


## Linking New Location

Steps:

1. Open Full Report in Rob's Sample
2. Excel PDF List - Copy PDF link (column K)
3. "Find" PDF link in Excel Sheet 3
4. Excel Sheet 3 (Column H) Production Link - Shows what the articles look like live
5. Excel Sheet 3 (Column I) Q2 - Staging Page
6. Excel Sheet 3 (Column J) Source Code / Edit Link
7. Edit New Link - Absolute Link
8. Excel PDF List - paste new link to "Converted_URL" (Column I)
9. Repeat for all rows highlighted during step 3


## High Level Tagging

EVERY POST SHOULD HAVE A TAG. IF IT DOESN'T FIND ROB

Apply tags for each article from the following list

* AI/Machine Learning
* Ad Blocking
* Ad Operations
* Ad Revenue
* Ad Sales
* Ad Technology
* Admin & Finance
* Administration
* Advanced TV
* Advocacy (also includes iab topic Public Policy)
* Affiliate Marketing
* App Marketing
* Audience Insights
* Audio
* Augmented Reality (AR)
* B2B
* Big Data
* Brand Insights
* Branded Content
* Building Brands In Digital
* Buying and Selling
* CCPA
* CaCPA
* California Privacy Act
* Certification
* Compliance
* Content Marketing
* Creative
* Cross-Screen
* Data
* Data Privacy
* Device Usage
* Digial Marketing & Media
* Digital Ad Operations
* Digital Attribution
* Digital Data Solutions
* Digital Media Buyers & Planners
* Digital Media Sales
* Digital Out of Home
* Digital Purchase Influence
* Digital Trends
* Digital Video
* Direct Brand
* Direct to Consumer
* Display
* Diversity & Inclusion
* Dynamic Creative
* Emerging Technologies
* FCC
* FTC
* GDPR
* Games
* Generational
* Global
* Government
* Guidelines
* HTML5
* Holiday Shopping
* IAB Education Foundation
* IAB Tech Lab
* iDiverse
* In-App Advertising
* Influencer Marketing
* LGBTQIA
* Law
* Learning
* Legal Affairs
* Legislation
* Local
* Location Data
* Long Tail Alliance
* Make Mobile Work
* Market Intelligence
* Measurement
* Measurement, Viewability and 3MS
* Measuring Ad Effectiveness
* Media Planning
* Mobile
* Mobile Apps
* Mobile Center Member Spotlight
* Mobile Data
* Mobile Web
* Multicultural
* Native Advertising
* Native Video
* OTT (Over-The-Top) Video
* Operations
* Parenting
* Playable Ads
* Podcast
* Privacy
* Programmatic
* Publisher Content Studio
* Purchase Intent
* Quality Assurance
* Regulation
* Rewarded Ads
* Rising Stars
* Self-Regulation
* Social Media (originally Social in IAB)
* TV
* Targeting & Measurement
* Tax
* Traffic Fraud
* Training and Seminars
* User Experience (UX)
* User Generated Content (UGC)
* Value Exchange
* Verification
* Video
* Virtual Reality (VR)
* Webinars
* White House

## Update all links so it points ot the new post

Go to [Rob will provide link](#) and assign a document to yourself
