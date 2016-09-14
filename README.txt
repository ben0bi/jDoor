jDoor Version 1.1.1-beta

jDoor is a jQuery-plugin for creating moveable windows which can be brought
from the background to the front and vice versa. The background windows will
be locked, only the one with the focus can be used.

jDoor is created by Beni Yager in 2016
twitter.com/ben0bi
benedictinerklosterbruder.blogspot.com
ben0bi.homenet.org

Internet Explorer is not supported, sorry.
But on Edge it works fine.

Not tested with Opera and Safari.

CHANGES:
1.1.1:
	-> Now uses cookies to save the window positions.
		You can turn cookies off by setting $.fn.jdoor.defaults.UseCookies to false BEFORE creating any windows.
1.1.0:
	-> jdCreateWindow has now a 'title' variable: The title of the window, shown in the top bar.
		Version + 0.1 because you need to rewrite your app and give a title on window creation.
	-> Updated Example.
	-> Updated documentation.
1.0.4:
	-> If you give a negative number as width or height by jdCreateWindow, 
		it will treat it as "max-height" instead of "height".
	-> Updated the example.
1.0.3:
	-> Fixed a critical width/height switching error.
1.0.2: 
	-> Created c4m theme (For the cinema4me website.)
	-> $('..').jdHTML does now return the html in the jdwindow-content div.
1.0.1:
	-> new Method: $('#targetwindow').jdHTML(html) 
		Sets the html content of a window. 
		Targetwindow must have the class jdwindow and include a div with the class jdwindow-content.

	-> new Method: $('#targetscreen').jdHideAllWindows()
		Hides all content with the class jdwindow in the given targetscreen.