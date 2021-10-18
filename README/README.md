DOCTYPE: READ-ME
 
 ,~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~,
{ Horiseon: Landing/Homepage v.10.14.21 }
 '~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~'
 
Welcome to the v.10.14.21 (October 14, 2021) release of the Horisean landing and home-page
READ-ME Document;
 
 
 ,~~~~~~~~~~,
{* Contents *}
 '~~~~~~~~~~'
 
  I  ) File Manifest
   
  II ) Changes from v.10.14.20
    i  . page content updates  
    ii . style updates
 
  III) Developer Notes and How-to
    i  . full-page <div> map
    ii . section-by-section formatting and corresponding style changes
 
  IV ) Acknowledgements
 
~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
 
 
 ,~-~~~~~~~~~~~~~,
{I) File Manifest }
 '~~~~~~~~~~~~~-~'
["#>":Folder , ">":File , "-":Tier 1]
 
<ROOT>Horiseon-refactored.home
 
   -  #>assets
               #>css
                     >style.css
               #>images
                     >benefits-1.png
                     >benefits-2.png
                     >benefits-3.png
                     >content-1.jpg
                     >content-2.jpg
                     >content-3.jpg
                     >hero.jpg
               
   -   >.gitignore
 
   -   >index.html
 
   -  #>README
                >README.md (you are here)
               #>README-Images
                     >Horiseon Home Page pt.1
                     >Horiseon Home Page pt.2
/ROOT>
 
~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
 
 
 ,~-~-~~~~~~~~~~~~~~~~~~~~~~,
{II) Changes from v.10.14.20 }
 '~~~~~~~~~~~~~~~~~~~~~~-~-~'
 
 
II>>>>>>>>>>>>>{^~
  (i) page content updates  ~^}
 
 
Folder:/Horiseon-refactored.home:
 
  *Folder Renamed:
    -Root-Directory name updated from
    "urban-octo-telegram"
    as in version 10.14.20 to
    "Horisean-refactored.home"
    as this name is more fitting for that which
    the directory describes and contains.
 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
File:~/index.html:
 
  *Head Meta-data Updated:
   -Added meta description and keyword tags to assist with
   search engine optimization and accessibility.
 
  *Head <title> Element Updated:
   -Updated the home page site-title from
   "website" to
   "Horiseon: Social Solution Services"
   as to reflect the organizations name and product/Services
   in the eyes of the browser tab and search engine crawler.
 
  *Body Comments Added:
   -Comments utilized in body of index.html in order to denote
   which part of the page a different element/section/or article
   belongs too as an added denotion measure; though like groups are
   still coded close together.  For the main portion of the page the
   comments also provide important formatting instructions for the different
   cards utilized in the separate "Homepage Descriptive Content" and
   "Benefits Sidebar" sections.
 
  *Body Spacing Added:
   -Spacing added between disparate sections so as to present code
   readable in a way more indicative to the front-end presentation.
 
  *Selector Removal:
  -The "class" selectors "header" and "footer" have been removed from the former
  <div> tags which have now been titled "<header>" and "<footer>" respectively.
  Corresponding changes can be found on the stylesheet and are explained further under
  the "~/assets/css/style.css" changes
 
  *Selector Addition:
   -Selector <id> added to the first card in the "Homepage Descriptive
   Content" section.  This introduces consistency with the formatting
   of the remaining two cards while also returning functionality to the
   "Search Engine Optimization" button in the Header's Navigation Section.                                                                                                                               
   
  *Header Upleveling:
   -Upleveled <h3> tags in the "Benefits Sidebar" section to maintain
   standards in regards to heading level as there is no <h2> element that
   is parent to "Benefits Sidebar".  Styling is maintained to match the
   mockup/original through the linked stylesheet and the particular trait:
   ".benefit-widget h2 {...; font-size: 1.17em; }"
   >Note: More information about this trait addition can be found in the
   "New Instructions Added" section under the "~/~/css/style.css" changes
 
  *<img>s Have Been Given "alt" Attributes:
   -All of the pages <img> tags have been given "alt" attributes; either descriptive text
   for the "Homepage Descriptive Content"'s <article>s or an empty "" value for the "Hero"
   and "Benefits Sidebar" sections.  This enhances accessibility by providing descriptive
   text in images that need it; and by telling screen readers that there is no text in images
   that won't.
 
  *<div> tags Converted/Updated:
   -All of page's <div> tags have been converted into semantic elements
   that reflect their content's purpose within the website.  This includes
   the introduction of <header> , <nav> , <section> , <article> , <aside> ,
   and <footer> elements; aiding site accessibility and differentiation
   for the parser and developer alike.
   >Note: Formatting of semantic tags explained in "III) User Notes and How-to"
 
  *Selector Consolidation:
   -selectors for mapping the stylesheet onto index.html have been consolidated
   from their previous naming convention to one that focuses
   more on page location/function; explained further under the "~/style.css" changes.
   >Note: Particular conversions and formatting explained in
   "III) User Notes and How-to"
 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
II>>>>>>>>>>>>>{^~
  (ii) style updates  ~^}
 
 
File:~/assets/css/style.css:
 
  *Body Comments Added:
   -Comments utilized in body of style.css in order to denote
   which part of the page a set of particular instructions-by-selector
   belong to as an added denotion measure; though like groups are
   still coded close together.  
   These divisions primarily match to the divisions demarcated by "index.html"'s
   notes and spacing; with an added divide between selectors for style-guides for the
   full-site, body, header, and footer;
   while every other element for the main-page's body styling is placed in a
   separate content divider.  This design was done with modularity and future
   expansion in mind; allowing for quick identification of the styleguides that
   would be reused in the  development of other pages on Horiseon's website.
 
  *Selector Styleguides Organized:
   -Advantage was taken of the conversion of multiple redundant instruction
   sets into singular common classes;
   as well as <div>s  being converted into semantic elements,
   to organize the Stylesheet into a format that best allows quick selector identification
   and style-guide reuse.
 
  *Selector Consolidation:
   -selectors for mapping this stylesheet onto "index.html" have been consolidated
   from their previous naming convention to a naming convention that focuses
   more on page location/function;
   This allows this style-sheet to be less dependent on its numerous previous reduncies
   and more capable of deployment in the creation of future page elements and new
   pages that will conform with the homepage's style-guide.
   >Note: Particular conversions and formatting explained in
   "III) User Notes and How-to"
 
  *Class Selector Conversion (header/footer):
   -the original class selectors for header and footer on this stylesheet have been
   updated to semantic selectors as the "header" and "footer" classes are no longer
   in use in "index.html"; their functionality now being handled by the former classes
   respective semantic elements (<header> and <footer>)
 
  *New Instructions Added:
   -The only "new" instruction added to any particular selector was the addition
   of the "font-size: 1.17em;" to the ".benefit-widget" classed objects found in
   the section labeled the "Benefits Sidebar" as mention under the changes for
   "index.html"
   >Note: This styling overrides the default h2 size (1.5em) for font in the
   "User Agent Stylesheet" and replaces it with the h3 sizing of 1.17em.  
   If you encounter any formatting errors verify proper function of your
   User Agent Stylesheet
 
Folder:~/assets/images:
   -image names converted much like class names in "index.html" to reflect-not their
   individualized message to consumers; but to reflect their location and purpose
   in the context of the page as a whole.
   >Note: Particular conversions and formatting explained in
   "III) User Notes and How-to"
 
~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
 
 
 ,~-~-~-~~~~~~~~~~~~~~~~~~~,
{III) User Notes and How-to }
 '~~~~~~~~~~~~~~~~~~~-~-~-~'
 
 
III>>>>>>>>>>>>{^~
  (i) full-page <div> map  ~^}
 
 
-As the <div>s have been converted to semantic tags that reflect an elements
particular place on the final presented page; it is more important to acknowledge
the exact formatting when making changes to the page; proper order of divisions:
 
<!DOCTYPE html>
 
0 )<body>
1 )     <header>
2 )         <h1>
3 )         <nav>
4 )             <ul>
5 )                 <li>
6 )                     <a>
7 )     <section class="hero">
8 )     <section class="content">
9 )         <article>
10)             <img>
11)             <h2>
12)                 <p>
13)     <section class="benefits">
14)         <aside>
15)            <h2>
16)                 <img>
17)                 <p>
18)     <footer class="footer">
19)         <h2>
20)             <p>
 
 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
III>>>>>>>>>>>>{^~
  (ii) section-by-section formatting and corresponding style changes  ~^}
 
 
<div>s 1-6/Page Header and Navigation:
 
  0)<header>
  1)          <h1><span id="seo"></span></h1>
  2)          <nav>
  3)              <ul>
  4)                  <li><a href="#[...section-name...]"></a></li>
  5)              </ul>
  6)          </nav>
  X)</header>
 
    0. <header> used instead of <div class="header"> as the semantic tag <header> can be used with no new code
    needed; just conversion of the original class selectors into semantic selectors; while providing enhanced
    accessibility.
 
    1. <span>s in the <h1> tagged header used to highlight the letters 'S,E, and O' in the page
     title "Horiseon" to id-select them with #seo for unique coloration and highlight the letter-play
     that highlights Horiseons services.
 
    1-2. <h1> represents page title on top-left of the page; <nav> and contents the navigation bar to the top-right
    <nav> contents use an <a> tag that href to the section on the page sharing the id element that follows the "#"
    in the href's <a> tag
    ex':
     <a href="#social-media-marketing"> directs to <article id="social-media-marketing">
    contents between the opening and closing <a> tag should also reflect the words in the
    "id" selector for front-end users.
 
 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
<div>s 7/Hero:
 
  0)<section class="hero" alt=""></section>
 
    0. The <div> section with the class "hero" was converted to a <section> element with the same class
    to enhance page accessibility and differentiation through the use of semantic tags while not
    requiring any other changes to the stylesheet.
 
 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
<div>s 8-12/Homepage Descriptive Content:
 
  0)<section class="content">
  1)          <article id="[...section-name...]" class= "card">
  2)              <img src="./assets/images/content-#.jpg" class="float-[direction*]" alt="[...alt-text for image...]" />
  3)              <h2></h2>
  4)                  <p></p>
  5)          </article>
  X)</section>
 
    0. The <div> section with the class "content" was converted to a <section> element with the same class
    to enhance page accessibility and differentiation through the use of semantic tags while not
    requiring any other changes to the stylesheet.
 
    1. The <div>s within <section class="content" have been converted into <article>s which semantically better
    represents these divisions of the homepage.  The new <articles>s have the same "id" values they had when they
    were <div>s; this allows the "href" attributes in the <a> tages in the <header> division of the webpage
    to have a direction to link to when their hyperlinks are activated.
 
    1. the "class" selector for the three <article>s in the "Homepage Descriptive Content" section have been
    converted into one "card" class; as the only function these disparit classes provided was styling; styling
    that all three happen to share.  by using one shared class the styling reduncies have been removed for these
    <article>s; their <h2>s; and their <img>'s on "style.css"
 
    2. image files have been formated such that they are names after their section lass and car order; so the image for the
    first card would have the src: "./assets/images/content-1.jpg" with each next picture having the next ordered number.
    *the class="float-[right/left]" determines whether the card will feature the picture and then the header and text (left)
     or the header and text and then the picture (right).  Formatting conventions for the page would dictate that each next
     "card" <article> alternate these <img> class values.
 
    2-4. It is critical in formatting these "card" <article>s that one follows the below format guide; which keeps
    the <article>'s image, and all of the <article>'s text (<h2> , <p>) in separate thematic subdivisions.
 
    Format Guide-
            <article>
        1:     <img>..~..</img>
        2:     <h2>..~..</h2>
        3:        <p>..~..</p>
            </article>
 
 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
<div>s 13-17/Benefits Sibebar:
 
  0)<section class="benefits">
  1)          <aside class="benefit-widget">
  2)              <h2></h2>
  3)                  <img src="./assets/images/benefits-#.png" alt="" />
  4)                  <p></p>
  5)          </aside>
  X)</section>
 
    0. The <div> section with the class "benefits" was converted to a <section> element with the same class
    to enhance page accessibility and differentiation through the use of semantic tags while not
    requiring any other changes to the stylesheet.
 
    1. The <div>s within <section class="benefits" have been converted into <aside>s which semantically better
    represents these divisions of the homepage.
 
    1. the "class" selector for the three <article>s in the "Benefits Sidebar" section have been
    converted into one "benefit-widget" class; as the only function these disparit classes provided was styling; styling
    that all three happen to share.  by using one shared class the styling reduncies have been removed for these
    <aside>s; their <h2>s; and their <img>'s on "style.css".  It was going to just be "benefit" but this was determined
    to be way too close to "benefits" so was changed to prevent future identification issues.
 
    3. image files have been formated such that they are names after their section lass and car order; so the image for the
    first card would have the src: "./assets/images/benefits-1.jpg" with each next picture having the next ordered number.
 
    2-3. It is critical in formatting these "benefit-widget" <aside>S that one follows the below format guide; which keeps
    the <asides> formatting order of 'header', 'image', and 'text'.
 
    Format Guide-
            <aside>
        1:     <h2>..~..</h2>
        2:        <img>..~..</img>
        3:        <p>..~..</p>
            </aside>
 
 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
<div>s 18-20/Footer and Acknowledgements:
 
  0)<footer class="footer">
  1)          <h2></h2>
  2)              <p></p>
  X)</footer>
 
    0. <footer> used instead of <div class="footer"> as the semantic tag <footer> can be used with no new code
    needed; just conversion of the original class selectors into semantic selectors; while providing enhanced
    accessibility.
 
    1-2. <h2> represents page title and branding above copyrite and acknowledgement; <p> represents said
    copyrite and acknowledgements below the branding.
 
~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
 
 
 ,~-~-~-~-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~,
{IV) Developer Notes and Acknowledgements }
 '~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-~-~-~-~'
 
 
 *This site is property of Vanderbilt Coding Web Development Bootcamp; Refactoring work done by Nicholas Holzer.
