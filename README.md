HTML 5
---------------------------------------------------------------------------------------------

    Hyper Text Markup Language

                                    SGML        Stand., General Markup Language
                                     (ML specifiction)
                                     |
                                     |
                                    ----------------------------
                                    |                          |
                                    HTML                      XML

    HTML was deviced to write formated documents that cna be hsoted on a http server and can be
    requested for and resposned back over HTTP protocol.

    Browser to parse an .html document and render the formatted content on the screen.

    Hyper Text
            Plain Text
            Images/Graphics
            Formated text
            Links

    Mark UP

            Vizag - the steel city - is my home town.

            She said to me "Visit Raman for the details on the project".


    HTML
            an html document composes of elements.
            each element is some content wrapped (marked around with) an open and close tag.
            each tag cna be supplied with additonal info using attributes.


            <p style="text-align:center">
                this is a para.
            </p> 

            This is a para element where <p> is an opening tag </p> is a closing tag
            and style is an attribute.

    HTML DOC

            <!doctype html>

            <html>
                <head>
                    <!--all meta data-->

                </head>
                <body>
                    <!-- contnet -->
                </body>
            </html>

    
    HTML basics
        heading,paragraphs and typology
    
        h1 h2 h3 h4 h5 h6           block elements
        p                           block elements
        b i u strong em             inline elements
        sup sub                     inline elements
        blockquote                  block element
        div                         block element
        span                        inline eleemnt

    HTML Lists

        ol          Ordered list
            type    attribute takes 1,a,A,I,i as values
        ul          Unordered list
            type    attribute takes dot,circle,square as values   

        li          list item is a sub-tag of ol and ul.

    HTML Tables    
        table                   to create a table
                border          attribute takes 1 to 5
                width           attribute takes a value in px/%/em/pt/in/cm
                heigth          attribute takes a value in px/%/em/pt/in/cm
                cellspacing     attribute takes a valeu in px/%/em/pt/in/cm and controls the spacing between two 
                                cells
                cellpadding     attribute takes a valeu in px/%/em/pt/in/cm and controls the spacing between the 
                                cell border and its content

        caption                 sub-element to give a heading to the table
        tr                      table row is a sub element representing one row
        th                      table hader cell, a sub-element of tr
        td                      table data cell, a sub-element of tr
                rowspan         attribute of th and td representing the number of rows to be occupied default is 1
                colspan         attribute of th and td representing the number of columns to be occupied default is 1
       
    HTML Media

        img         inline element that injects an image into the page
             src    attribute of img tag to hold the relative or absolute or virtual path 
                    of the image

        audio       inline element to inject an audio
        video       inline element to inject a video
        source      sub-element of audio and video to supply the audio file or video file
                    a single audio or video element can house anynumber of source tags
                    each represeting a different format of audio or video.
            src     attibute of source to hold the relative or absolute or virtual path 
                    of the audio or video file

        iframe      used to embed an external web page into our own web page.
            src     attribute to hold the web address of the webpage you wish to embed.

    HTML Links
        a           amchor tag 
            href    attribute takes the target file path.
            target  attribute takes _self/_blank/iframeName

    HTML Form Elements
        form                is used to group a set of fields that have to be submitted to a server program.
            action          attribute takes the path of the server program to which the data has to be submitted
            method          attribute that takes GET/POST
        
        label               used to carry a text related to a field like field names
            for             attribute takes th id of the input element to which the label is related to.

        input               used to create a form field control that enable inputting data
            type            text
                            file
                            password
                            checkbox
                            radio

                            number
                            range
                            decimal
                            email
                            date
                            datetime-locale
            
            id              attribute is used to give an id to the input element.
            name            attribute is sued to give a field name that is carried along with its value to the server.
            value           attribute takes the initial vbalue of the field

            required        attribute ensures that the field is given a value mandatly
            min             attribute that takes a minimum possible value for type="number/decimal/date"
            max             attribute that takes a maximum possible value for type="number/decimal/date"
            minlength       attribute that takes a minimum length of the value while type="text"
            maxlength       attribute that takes a maximum length of the value while type="text"
            pattern         attribute that takes a reglar expression to validate the value while type="text"

        textarea            used to accpet multi line text
        
        select              used to create a drop-down or a list box
            multiple        attribute makes the drop-down into a list enabling multiple option selection
         option             is a sub-element of select used to provide the options
            value           attribute of option tag that takes the value to be submitted if this option is selected

        button              used to create a push button
            type            submit      (defualt)
                            reset
                            button

    HTML Layouts and sematic elements

        <header>    - Defines a header for a document or a section
        <nav>       - Defines a set of navigation links
        <section>   - Defines a section in a document
        <article>   - Defines an independent, self-contained content
        <aside>     - Defines content aside from the content (like a sidebar)
        <footer>    - Defines a footer for a document or a section
        <details>   - Defines additional details that the user can open and close on demand
        <summary>   - Defines a heading for the <details> element
        <figure>    - Defines a self-contained content, like illustrations, diagrams, photos, code listings..etc
        <figcaption>- Defines a caption for a <figure> element.
        <time>	    - Defines a date/time


    HTML entities

        Result	        Description	            Entity Name	    Entity Number
        =============================================================================
        non-breaking    space	                &nbsp;	        &#160;
        <	            less than	            &lt;	        &#60;
        >	            greater than	        &gt;	        &#62;
        &	            ampersand	            &amp;	        &#38;
        "	            double quotation mark	&quot;      	&#34;
        '	            single quotation mark 	&apos;      	&#39;
        ¢	            cent	                &cent;	        &#162;
        £	            pound	                &pound;	        &#163;
        ¥	            yen	                    &yen;	        &#165;
        €	            euro	                &euro;	        &#8364;
        ©	            copyright	            &copy;	        &#169;
        ®	            registered trademark	&reg;	        &#174;
    
CSS 3 
-------------------------------------------------------------------------------------
    CSS 3 - Intro
    -----------------------------------

        Cascading Style Sheet

        purpose is to provide styling to an html document.

        + CSS offers common uniform properties unlike html
        + CSS can provide styling across grouped elements.
        + CSS can isolate styling from content. It adds to maintainability.
        
        Inline Style Sheet

            it is applied using 'style' attribute.

            <tagName style="css-property:value;css-property:value;">
                content
            </tagName>

        Embeded Style Sheet

            it is applied using a tag called <style></style>, style elements
            is a sub-element of <head></head>

            <head>
                <style>
                    selector {
                        css-property:value;
                        css-property:value;
                    }
                </style>
            </head>

            selector is a string that qualfies the elements to be applied with the style.

            1. Tag Name
                    each tag name itself is a selector.
                    
                    tagName{
                        css-property:value;
                    }

            2. Attribute
                    attribute selector groups elements having the mentioned attribute.
                    
                    [attributeName]{
                        css-property:value;
                    }
                    
                    [attributeName=""]{
                        css-property:value;
                    }

            3. Class

                    is any usr defiend string. that should start with dot(.)
                    to apply the class on a element the element class attribute 
                    should be assigned with the class name.

                    .className{
                        css-property:value;
                    }

                    <tagName class="className">
                    </tagName>
            4. Id
                    if a style swhould be applied to an elemnt hving 
                    a specific id, then id selector is sued.

                    #id{
                        css-property:value;
                    }

            5. Psuedo


        External Style Sheet

            style is defiend in a seperate file with extension .css
            and that cna be linked to any number of html pages using
                
                <link href="fileName.css" rel="stylesheet" />


    CSS - unit of measure
    ------------------------------------

        absolute		(irrespective of screen size)
            in
            mm
            cm
            pt		1 in = 72 pt
            pc		1 in = 6  pc   1 pc = 12 pt
        
        relative 	(to screen size)
        
            px
            
            %
            
            em			relative the font-size
                        1 em = complete font-size
                                            
                        font-size: 12pt;
                        width: 8em;	8*12pt = 96pt;
                        
            vh			1% of viewport height
            vw			1% of viewport width
            vmin		min of vh or vw


    CSS Box Model Properties
    -----------------------------------
        margin
        margin-top
        margin-bottom
        margin-left
        margin-right

        border              border-size border-style border-color
        border-top
        border-bottom
        border-left
        border-right

        padding             space between the contetn and the elemnt border
        padding-top
        padding-bottom
        padding-left
        padding-right

        border-radius       radius of the corners of the element
        border-top-left-radius
        border-top-right-radius
        border-bottom-left-radius
        border-bottom-right-radius

        width
        height
        min-width
        min-height
        max-width
        max-height

        display             inline/block/inline-block

        position            relative / absolute

        top
        left
        bottom
        right
        z-index

    CSS background color and image related properties
    ----------------------------------------------
        background-color
        color
        background-image
        background-repeat       no-repeat/repeat/repeat-x/repeat-y
        background-position
        background-attachment    fixed/scroll
              
    CSS font related properties
    -----------------------------------
        font-family
        font-size
        font-variant		normal or small-caps
        font-weight			bold or bolder or boldest 
                            or any number like 300,400,500..etc
        font-style			italic or oblique
        
    CSS Text related Proeprties
    -----------------------------------
        color
        direction
        letter-spacing
        word-spacing
        text-align
        text-indent
        text-decoration		none | underline | line-through | overline
        
    table related css prperties
    ------------------------------------
        border-collapse			collapse or seperate
        border-spacing
        caption-side			top left right bottom
        
    CSS list related properties
    ----------------------------------

        list-style-type			disc	circle	square	none	for ul
                                decimal							for ol
                                decimal-leading-zero	
                                lower-alpha
                                upper-alpha
                                lower-roman
                                upper-roman
        list-style-position		outside or inside
        list-style-image:		url('imgs/note.png')
        marker-offset
        
  
    controlling scroll bars
    ------------------------------------
        
        overflow
                    visible
                    scroll
                    auto
                    hidden
    CSS Operators
    -------------------------------------
        s1		applies to elements that have s1 as tag name
        .s1		applies to elements that have s1 as class
        #s1		applies to elements that have s1 as id

        s1,s2	applies to elements that match both selectors
        s1 s2	applies to all elements that match s2 and are inside s1
        s1>s2	applies to all elements that match s2 whose parent is s1
        s1+s2	applies to all elements that match s2 and are immediately after s1
        s1~s2	applies to every element that match s2 and is preceded by s1

                        applies to all elements that have
                        ------------------------------------
        [s1]			 s1 as attribute
        [s1='v1']		 s1 attrib with v1 value
        [s1~='v1']		 s1 attrib value containes word v1
        [s1*='v1']		 s1 attrib value containes word v1
        [s1!='v1']		 s1 attrib value not equal to v1
        [s1^='v1']		 s1 attrib value starts with the word v1
        [s1$='v1']		 s1 attrib value ends with the word v1

        Psuedo selectors
        ----------------------------------------------------------------------------
        input:enabled	Selects every enabled <input> element
        p:first-child	Selects every <p> element that is the first child 
                        of its parent
        p::first-letter	Selects the first letter of every <p> element
        p::first-line	Selects the first line of every <p> element
        p:first-of-type	Selects every <p> element that is the first <p> 
                        element of its parent
        input:focus		Selects the input element which has focus
        a:hover			Selects links on mouse over
        input:in-range	Selects input elements with a value within a specified range

        input:indeterminate		
                        Selects input elements that are in an indeterminate state

        input:invalid	Selects all input elements with an invalid value
        input:optional	Selects input elements with no "required" attribute

        p:last-child	Selects every <p> element that is the last child of its parent
        p:last-of-type	Selects every <p> element that is the last <p> element of its parent

        a:link			Selects all unvisited links
        :not(p)			Selects every element that is not a <p> element
        p:nth-child(2)	Selects every <p> element that is the second child of its parent
        p:nth-last-child(2)	
                        Selects every <p> element that is the second child of its parent, 
                        counting from the last child

        p:nth-last-of-type(2)	
                        Selects every <p> element that is the second <p> element of its parent, 
                        counting from the last child
        p:nth-of-type(2)	
                        Selects every <p> element that is the second <p> element of its parent
       



