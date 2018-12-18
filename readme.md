# Migrate PDF Content

[2018-12-12 Updates](https://github.com/dabobert/iab_conversion#2018-12-12-updates)

[Tags Rob Didn't Create](https://github.com/dabobert/iab_conversion/wiki/Tags-Rob-Didn't-Create)

[Video](https://bluejeans.com/s/h93V4)

[Login Page](https://iabstaging.wpengine.com/wp-login.php?itsec-hb-token=iabadmin)


[Original page](https://iab.com/insights/themobileidguide/)

[Original PDF](https://www.iab.com/wp-content/uploads/2017/06/Mobile-Identity-Guide-for-Marketers-Report.pdf)

[Rob's sample migration](https://iabstaging.wpengine.com/insights/themobileidguide/)

## 2018-12-17 Updates

### Cobraded images

Co-branded logos should have the class `iab_cobranded` like

```
<img src="spotify_logo.png" class="iab_cobranded" />
```

### Using Microsoft Word to convert PDFS

1: open pdf as word file
2: save each image, and then delete each image (will be used for uploading)
3: select all text convert it to black
4: copy and paste all content (it now has no images, and is all black) into wordpad
5: Use word pad to make sure that the flow of paragraphs is correct
6: You will need to:
  * recreate lists
  * insert images



## 2018-12-12 Updates

### Publishing Content

After your article has been approved, the following steps should be performed

1. **PUBLISH** the article
1. Copy and paste the final URL into the [Spreadsheet](https://docs.google.com/spreadsheets/d/1J8e9WzqxtfqzDAWA08nQx70yGEfFO5_7dq_1shs4YuY/edit#gid=0)
1. Use this Published URL to replace the links to the orignal PDF


### Add Insight Types

Make sure to add an insight type to all content added.  

* One-Sheet
* Infographic
* Case Study
* Research
* White Paper

The insight types menu is below topics 

<img src="https://s3.us-east-2.amazonaws.com/misc-iab-files/iab_conversion-insight_types.png" height="50%" width="50%" />


### Creating table of contents

To create table of contents you ONLY need to create the headings within the document.

Use `<h3 class="toc">Title</h3>` for main headings.

Use `<h4 class="toc">Sub-Title</h4>` for sub-headings.



There will be code that will convert these headings into links, as such there is no need to create the headings manually ie doing the following

```
Transcoding Video............................6
```

is both

1. not needed, because the code will be creating the links
1. incorrect because the page numbers do not translate to a web page


### Download Links

Links to download pdf files like the one here

`<a class=" pdf_download_link" href="http://www.iab.com/wp-content/uploads/2017/06/VerticalVideo-Research.pdf">Download</a>`

should be at the should be at the **BOTTOM** of the page.  This ensures that the first letter of the article will be copy and not download as shown in the image below

<img src="https://misc-iab-files.s3.amazonaws.com/download_captilized_letter.png" width="50%" height="50%" />

Again it should NOT look above

## Select an article to convert

Go to [https://goo.gl/c2yQRF](https://goo.gl/c2yQRF) and assign a document to yourself

IAB articles are top priority 

## Login into WP Admin


[Login](https://iabstaging.wpengine.com/wp-login.php?itsec-hb-token=iabadmin) into the WPAdmin area


## Create a new `Insight` for the 

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


`<img src="bla.jpg" id="iab-hero-image">`

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


## Style Guide

* Downnload Link
* Headers are tagged with h3/h4 AND are lines by themsleves
* Captions/comments aere italicized
