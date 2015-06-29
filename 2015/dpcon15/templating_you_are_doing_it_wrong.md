Nikolas Martens - "Templating - you're doing it wrong"
######################################################

At first, templating seems like a good idea: Separate logic from presentation by putting all HTML documents in in their
own files. But we still need to glue them to the logic of our application somehow so we use a specialized mark-up 
language and a matching text-manipulating interpreter to render them. And since there are already at least five 
different languages in any web application, nobody minds another one or the fact that you can't render a template 
without having the whole application running.

But this is an unnecessary burden since there already is a widely used and proven mark-up language in every HTML 
document: the HyperText Markup Language. In this talk, I'm proposing an new approach to writing templates for web 
applications, called Template Animation, that leverages the capabilities of HTML to create highly maintainable 
templates, requiring no tools besides the browser for development and testing.

Sources
=======

 * Talk <>
 * Blog <http://rtens.org/>
 * Twitter <http://twitter.com/rtens_>
 * Github <http://github.com/rtens>

Notes
=====
 
 * Source <http://www.workingsoftware.com.au/page/Your_templating_engine_sucks_and_everything_you_have_ever_written_is_spaghetti_code_yes_you>
 * Templating: Maintenable == Runnability not Readability
 * Runing the template in the Browser is ugly
 * Do it better with a clickable prototype
   * html + view model --animate--> application html
   * Tool for this <https://github.com/watoki/tempan>

 * Template engines do text manipulation
 * Template animation do dom manipulation
   * Matching the ViewModel with HTML via DOM-API || Css selector || Annotation in HTML
   * Matching via Annotation via property attribute

