# Media-Query
---------------------

Media queries are useful when you want to modify your site or app depending on a device's general type (such as print vs. screen) or specific characteristics and parameters (such as screen resolution or browser viewport width).
-----------------------------------------------
Media queries are used for the following:
--------------------------------------------
To conditionally apply styles with the CSS @media and @import at-rules.
To target specific media for the <link>, <source>, and other HTML elements.
To test and monitor media states using the Window.matchMedia() and MediaQueryList.addListener() JavaScript methods.
Note: The examples on this page use CSS's @media for illustrative purposes, but the basic syntax remains the same for all types of media queries.
--------
<h2> Syntax </2>
------
A media query is composed of an optional media type and any number of media feature expressions. Multiple queries can be combined in various ways by using logical operators. Media queries are case-insensitive.

A media query computes to true when the media type (if specified) matches the device on which a document is being displayed and all media feature expressions compute as true. Queries involving unknown media types are always false.
-----------------------------------------------------
Note: A style sheet with a media query attached to its <link> tag will still download even if the query returns false. Nevertheless, its contents will not apply unless and until the result of the query changes to true.
-----------------------------------------------------
Link to sectionMedia types
--------------------------------
Media types describe the general category of a device. Except when using the not or only logical operators, the media type is optional and the all type will be implied.
------------------------
all
Suitable for all devices.
print
-----
Intended for paged material and documents viewed on a screen in print preview mode. (Please see paged media for information about formatting issues that are specific to these formats.)
screen
------
Intended primarily for screens.
speech
-------
Intended for speech synthesizers.
Deprecated media types: CSS2.1 and Media Queries 3 defined several additional media types (tty, tv, projection, handheld, braille, embossed, and aural), but they were deprecated in Media Queries 4 and shouldn't be used. The aural type has been replaced by speech, which is similar.
Link to sectionMedia features
Media features describe specific characteristics of the user agent, output device, or environment. Media feature expressions test for their presence or value, and are entirely optional. Each media feature expression must be surrounded by parentheses.
