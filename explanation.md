#Web Browsers

###Introduction
Web browsers are software applications designed to enable users to access information resourses available on the world wide web. Browsers present the resource the user chooses by requesting it from the server and displaying it in the browser window.
##Architecture of a Browser

The components comprising a browser are:

__1.User interface(UI)__: This is comprised of everything in the browser excluding the window where the requested page is viewed. This includes: the next and back buttons,the home button,the refresh and stop button, the bookmarks bar and the address bar.

__2.Browser engine__: This code communicates inputs of the UI to the rendering engine.

__3.Rendering engine__: Parsing HTML and CSS the displaying the requested content on the screen.

__4.Networking__: A platform independent code which performs network calls such as HTTP requests.

__5.UI backend__: Drawing basic widgets onthe browser such as combo boxes and windows. It exposes a generic non platform specific interface underneath which it uses Operating System (OS) UI methods.

__6.Javascript interpreter__: Parsing and executiong javascript code.

__7.Data storer__: A persistent layer which store data such as cache and cookies locally.

##The Rendering Engine
It displays requested content on the screen which can be in the form of HTML and XML documents.Oher documents such as PDF can be viewed using plug-ins and extensions.

Different browsers use different redering engines: Chrome and Opera(from version 15) use Blink, Safari and Chrome(on iPhone) use Webkit, Firefox uses Gecko, Internet Explorer uses Trident and Edge uses EdgeHTML.

###The Main Flow

The basic flow of the rendering engine occurs in four stages:

__1.Parsing HTML to construct the DOM tree.__

The rendering engine gets data from the network layer usually in 8 kB chunks. It parses the HTML documents and converts them to DOM nodes to construct the content/DOM tree. 

__2.Rendering tree construction.__

The engine parses style data both in external CSS files and in style elements. The render tree is created using DOM nodes and the parsed style data.

__3.Layout of the render tree.__

Each node of the render tree is given the exact coordinates where it should appear on the screen.

__4.Painting the render tree__

The render tree is traversed and each of its nodes is painted using the UI backend component.

_Sources_: *[engineers' garage](http://www.engineersgarage.com/articles/web-browsers-what-is-web-browser-working)
         *[html5 rocks](http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/)
         *[dzone](https://dzone.com/articles/how-browsers-work-behind)
         *[slideshare](http://www.slideshare.net/manishtrivedi/how-browser-work)


