# Guidelines

Xenko users will be reading your articles to learn about the engine in their every day work. 
Your goal is to write pages easy to understand and that are accessible to all. 
To help you in your quest and to have an unified documentation easy to use,
we ask you to follow to the below Guidelines when writing.

* [Writing Style](#Style)
  * [Conversation Tone](#Tone)
  * [Second Person](#Person)
  * [Active Voice](#ActiveVoice)
  * [Simple Vocabulary](#SimpleVocabulary)
* [Pages Content](#PagesContent)
  * [Getting Started Pages](#GettingStarted)
  * [Samples & Tutorials Pages](#SamplesTutorials)
  * [HOWTO Pages](#Howtos)
  * [Section Header Pages](#SectionHeader)
  * [Overview Pages](#Overview)
  * [Reference Pages](#Reference)
  * [Avoid Long Explanations](#LongExplanations)
  * [Use Images & Videos](#UseImagesVideos)
* [Pages & Files Structure](#FilesStructure)
  * [Pages Hierarchy](#PagesHierarchy) 
  * [Pages Order](#PagesOrder)
  * [Files Hierarchy](#FilesHierarchy)
  * [Files Name](#FilesName)
* [Formatting](#Formatting)
  * [Definitions](#Definitions)
  * [Page References](#References)
  * [Related Topics](#RelatedTopics)
  * [API References](#APIReferences)
  * [Code References](#CodeReference)
  * [Placeholders](#Placeholders)
  * [Labels](#Labels)
  * [Remarks](#Remarks)
  * [Notices](#Notices)
  * [Platform Notices](#PlatformNotices)
  * [Media](#Media)
    * [Videos](#Videos)
    * [Images](#Images)
    * [Diagrams](#Diagrams)
  * [Tables](#Tables)
  * [Lists](#Lists)
  * [Headers](#Headers)
  * [Letter Capitalization](#Capitalization)
  
Note: The following directions are just guidelines not rules. 
If they are not appropriate to your specific use-case, feel free to ignore them.

# <a name="Style"> Writing Style

## <a name="Tone"> Conversation Tone

> **Appropriate**
> 
> We want our documentation to have a conversational tone. You should feel as though you
> are having a conversation with the author as you read any of our tutorials or explanations.
> Your experience as a reader should be informal, conversational, and informative. You should
> feel as though you are listening to the author explain the concepts to you.
> 
> **Inappropriate Style**
>
> One might see the contrast between a conversational style and the style one finds with
> more academic treatments of technical topics. Those resources are very useful, but the authors
> have written those articles in a very different style than our documentation. When one reads
> an academic journal, one finds a very different tone and a very different style of writing.
> One feels that they are reading a dry account of a very dry topic.  

The first paragraph above follows our recommendation conversational style. The second
is a more academic style. You see the difference immediately. 

##  <a name="Person"> Second Person

> **Appropriate**
> 
> You should write your articles as though you are speaking directly to the reader. 
> You should use second person often (as I just have in these two sentences). 
> 2nd person doesn't always mean using the word 'you'. Write directly to the reader. 
> Write imperative sentences. Tell your reader what you want them to learn.
> 
> **Inappropriate**
> 
> An author could also choose to write in 3rd person. In that model, an author must find 
> some pronoun or noun to use when referring to the reader. A reader might often find 
> this 3rd person style less engaging and less enjoyable to read.

The first paragrah follows our recommended style. The second uses 3rd person. 
Please write in second person. You probably found that much easier to read.

##  <a name="ActiveVoice"> Active Voice

Write your articles in active voice. Active voice means that the subject of 
the sentence performs the action (verb) of that sentence. It contrasts with passive voice, 
where the sentence is arranged such that the subject of the sentence is acted upon. 
Contrast these two examples:

> **Appropriate**
> 
> The compiler transformed source code into an executable.

> **Inappropriate**
> 
> The source code was transformed into an executable by the compiler.

The first sentence uses active voice. The second sentence was written in passive voice. 
(Those two sentences provide another example of each style).

We recommend active voice because it is more readable. Passive voice can be more difficult to read.

##  <a name="SimpleVocabulary"> Simple Vocabulary

Keep in mind that Xenko users are not all native English speaker when you write your articles.
Your audience is international and they probably don't have the vocabulary you have.

As a general rule try to *target a 5th grade reading level" when you write.

#  <a name="PagesContent"> Pages Content

This documentation is composed of different types of pages. The expected content and layout
of the page directly depends on the type. Before writing your article, start by identifying the 
type of page you are targeting, then follow the below templates for content and layout.

In addition to content and layout guidelines based on the type of page, we finish this section 
with a few generic recommendations for the content.

##  <a name="GettingStarted"> Getting Started Pages
##  <a name="SamplesTutorials"> Samples & Tutorials Pages
##  <a name="Howtos"> HOWTO Pages
##  <a name="SectionHeader"> Section Header Pages
##  <a name="Overview"> Overview Pages
##  <a name="Reference"> Reference Pages
##  <a name="LongExplanations"> Avoid Long Explanations

Long explanation are quite indigestible for the reader. Most of the time, he simply skips them.
If not, he is not able to remember the essential point of the explanation. 

To avoid this, try to never explain more than one concept in a simple paragraph.
Try to keep your explanation short and simple and when possible add an image or a diagram 
that corresponds to the concept next to your text.

This guideline is even more important for Getting Started, Samples, Tutorials and HOWTO pages,
where the text should correspond more to instructions than explanations about Xenko concepts.
In those pages, you should either try to explain the concept in a simple lline or replace the
explanation by a reference to the page dedicated to the concept.

##  <a name="UseImagesVideos"> Use Images & Videos

As much as possible add images or videos to accompany your explanation. This helps the reader a lot.

Also whenever it makes sense, we recommend you to use small videos instead of images. 
We believe that the time where we had to use diagrams with lots of arrows going in all directions
because videos were too heavy is over. Nowadays Internet connections and compression algorithms 
are good enough to include short videos in the documentation and increase even more the ease of
understanding.

#  <a name="FilesStructure"> Pages & Files Structure

The hierarchy of the documentation pages is specified in the [manual/toc.md](manual/toc.md) file
and is independent from the file hierarchy of this repository. For example, a single article can
be added several times at different location in the documentation if needed. Nevertheless for ease
we ask you to try to keep the same hierarchy between the documentation pages and this
repository files.

To add a new page in the documentation, just add a new entry at the appropriate place in the 
[toc](manual/toc.md) file.

## <a name="PagesHierarchy"> Pages Hierarchy

As a general rule, we want to avoid deep hierarchies for the ease of navigation. 
As much as possible we recommend you not to go beyond 4 levels of depth.

> Getting Started
>   - Common Topic
>   - Targeted Audience
>      - Topic
> Samples & Tutorials
>   TODO decide hierarchy
> Section Header
>   - Overview
>   - Topic
>   - Sub-Category
>     - Sub-Topic
>   - HOWTO
>     - Do something

Page naming conventions:
* No prefix need to be added before the Overview and HOWTO pages ('Overview' and not 'Graphic Overview')
* The name of the pages under the HOWTO folder should start with a verb and describe an objective ('Activate post-effects to your game', etc)

## <a name="PagesOrder"> Pages Order

Documentation pages don't necessary need to be alphabetically ordered.

As a general rule, order your new pages as follow:

1. Chronologically when there is a chronological order (Getting started / tutorial pages)
2. Most important subjects first (Overview pages -> References pages -> HOWTOs) 
3. When pages have the same importance, order them alphabetically.

## <a name="FilesHierarchy"> Files Hierarchy

Article files should be organized into folders. As much as possible we will try to respect the
same hierarchy as the documentation. Files corresponding to section header should be included at the 
top of the folder having the same name and be named 'index.md'.

Media files (images and videos) referenced in articles should be placed in a dedicated folder
named 'media' and put next to the referencing articles.

Code sample files (C#, scripts, etc) referenced in articles should be placed in a dedicated 
folder named 'code' and put next to the referencing articles.

Hierarchy example:

> Graphic
>   - index.md
>   - Overview.md
>   - media
>     - OverviewImage1.png
>     - OverviewImage2.png
>     - OverviewVideo2.mp4
>   - PostEffects
>     - index.md
>     - media
>       - posteffectImage1.png
>     - code
>       - posteffectCode.cs

## <a name="FilesName"> Files Name

As much as possible, you should give explicit and human-understandable names to files.

Our recommendations are the following:
- Section Header files should always be named 'index.md'
- Article files should be named using the main title of the page (without spaces)
- Media files should have a simple name corresponding to the content of the file

Examples:
> **Appropriate**  
> index.md  
> PointLight.md  
> PointLightDiagram.png  
>
> **Inappropriate**  
> GraphicsIndex.md  
> PointLightFile1.md  
> Img20150902.png  

#  <a name="Formatting"> Formatting
##  <a name="Definitions"> Definitions

TODO Pierre Explanations

TODO Virgile styling

##  <a name="References"> Page References

TODO Pierre Explanations

## <a name="RelatedTopics"> Related Topics

To encourage readers to learn more about a topic and also to ease their navigation,
we recommand you as much as possible to add links to related topics at the bottom of your articles.

For this use the AAA(TODO Virgile) style, as follow: 
> TODO Virgile  
> TODO Virgile  
> TODO Virgile  

## <a name="APIReferences"> API References

A link to the API reference should be added for EACH mention of an API class, interface, function, etc.
To avoid to add too many times the same links, you can replace the function name by an action verb.

Adding a link to a reference API can be done the following way:
> @'MyNamespace.MyClass.MyFunction'

Example:
```
Use the @'SiliconStudio.Xenko.Audio.SoundEffectInstance.Play' function start playing a sound.
Playing an ongoing sound has no effect. Playing a stop sound restart the sound from beginning.
```

## <a name="CodeReference"> Code References

Code samples should be as small as possible, well commented and be properly formatted when included. 
There are two different ways to insert some code in your article. First add the code content directly in your 
article with the proper formatting or add a reference to an existing code file. 
We recommend you to add the code sample directly in your article except when the code sample is used
in several different places. In that case we recommend you to use a reference to a code file.
It can be much more efficient in term of maintenance.

Example:
> **Code directly included in the article**
> 
> \`\`\`cs  
> Asset.Unload(asset);  
> \`\`\`
>
> **Reference to an external code file**  
> \[\!code-csharp\[Main\]\(index.cs?start=5&end=9\)\]  // add line 5 to 9 of file index.cs


## <a name="Placeholders"> Placeholders

For ease of understanding make all placeholders start by 'My'.

Example:
> Content.Load("MyFolder/MyAsset");

## <a name="Labels"> Labels

Labels are optional info displayed at the top of the page so that readers can quickly understand intended target audience.

Please place them right after the top-level title.

There are several kinds of labels:

* Level (Beginner, Intermediate, Advanced) with `label-doc-level`
* Audience (Artist, Programmer, Designer) with `label-doc-audience`
* Platform (iOS, Android, etc...) with `label-doc-platform`

Example:
```
# Title

<span class="label label-doc-level">Beginner</span>
<span class="label label-doc-audience">Artist</span>

## Overview

Lorem ipsum...
```


## <a name="Remarks"> Remarks

Whenever you have explanations that is not necessary for the understanding of a concept but that
can be very useful in application, add them as remarks so that the reader knows that it is extra information
that can be skipped depending on its objective. We provide several types of remarks such as notes, warnings and
tips to give an addition clue to the reader on what kind of extra information he is going to find.  

You can add note, tip and warnings using the following syntax:

```
> [!NOTE]
> Some useful notes
```

Available types:
* NOTE
* TIP
* WARNING

Note that current styling will be improved.

## <a name="Notices"> Notices

TODO Pierre Explanations

TODO Virgile styling

## <a name="PlatformNotices"> Platform Notices

When there are explanations, notices or remarks that are specific to a given platform, you should
use the following formatting style to show the reader that the section can be skipped depending on 
the targeted platform.

TODO Virgile styling Android/iOS + example

## <a name="Media"> Media

You can add media content to your articles using the following syntax:
> \!\[Graphics Compositor Diagram\]\(media/graphics-compositor.png\)  

'Graphic Compositor Diagram' is the message displayed as fall-back if the image file can't be find.
'media/graphics-compositor.png' is the relative path to the file.

For each media file added, we kindly ask you to always include the 'source' file used to create 
your media file next to it. This will allow us to quickly update the images, diagrams and videos 
after some changes happen on the engine side. By source files we mean photoshop files, visio files, 
adobe premiere files, etc. When you create your media, try as much as possible to use either free
or mainstream tools.

Avoid to resize the source data when you create your media. Even if your media needs to be scaled down
to fit the screen, avoid to create scaled-down media by yourself. Instead keep your image in the
original resolution and let the documentation system automatically adapt it for the user. We are asking 
this because at some point we may decide to change the width of our documentation or to provide 
a way to zoom into images. The only exceptions to this are heavy videos. We would like you to create 
a lighter version of the videos to speed up the loading of the pages.

### <a name="Videos"> Videos

As much as possible, we ask you to use the **MP4** format and the **H265** encryption for videos.

Recommenced software to edit the videos is Adobe Premiere.

### <a name="Images"> Images

We ask you to use the **JPEG** format for heavy high resolution images to reduce the load time and
and the **PNG** format all the others (probably most of the images).

For the source files, we prefer the following formats: Photoshop, GIMP, Paint.net.

### <a name="Diagrams"> Diagrams

Diagrams should be rendered as **PNG**. The source file can be done with Visio or standard image editing tools.

## <a name="Tables"> Tables

You can add tables to the documentation by following the markdown syntax. Tables can improve the
way information is display but sometimes does not properly scale down. So be sure to try your page
on small resolution screen like Smartphones before submitting your page.

## <a name="Lists"> Lists

When possible prefer a short phrase than a full sentence for each item of a list. This simplifies and
speeds the reading up. Start each item with a capital letter.

When showing a step by step process or when order matters use ordered list rather of bullet points.

Example. 
> **Appropriate**
> 
> How to use lists:
> - Capitalize each first letter
> - Write short phrases
> 
> **Inappropriate**
> 
> How NOT to use lists:
> - You should capitalize the first letter of each item.
> - You should write short phrases

## <a name="Headers"> Headers

The markdown '#' mark should be used to make headers. Only top title of the page should have the h1 style.
All other titles are sub-titles and should be formated into h2+.

Example
> \# Page Top Title: How to write headers.  
> \___  
> \## This is a sub-folder  
> \### This is a sub-sub-folder  
> \### This is another sub-sub-folder  
> \## This is another sub-folder  

## <a name="Capitalization"> Letter Capitalization

When a title is close to a full sentence you should only capitalize first letter of first work.
When a title is just composed of a few words (1 to 5) you should capitalize the few letter of each 
word.

You should NEVER fully capitalize a word inside a sentence except when you want to strongly insist on 
a fact. Words commonly used for this are: ONLY, DO NOT, YES, NO, MAKE SURE TO, BE CAREFUL (TO/ OF).
