# focus on the user

How much better would social search be if Google surfaced results from all across the web? The results speak for themselves. We created a tool that uses Google’s own relevance measure—the ranking of their organic search results—to determine what social content should appear in the areas where Google+ results are currently hardcoded.

All of the information in this demo comes from Google itself, and all of the ranking decisions are made by Google's own algorithms. No other services or APIs are accessed.

## How It Works
When you search for "cooking" today, Google decides that renowned chef Jamie Oliver is a relevant social result. That makes sense. But rather than linking to Jamie's Twitter profile, which is updated daily, Google links to his Google+ profile, which was last updated nearly two months ago. Is Google's relevance algorithm simply misguided?

No. If you search Google for Jamie Oliver directly, his Twitter profile is the first social result that appears. His abandoned Google+ profile doesn't even appear on the first page of results. When Google's engineers are allowed to focus purely on relevancy, they get it right.

So that's what our "bookmarklet" does. It looks at the three places where Google only shows Google+ results and then automatically googles Google to see if Google finds a result more relevant than Google+.

For more info, read [focus on the user](http://www.focusontheuser.org/).

## Bookmarklet

Drag this button to the browser's bookmarks toolbar in Chrome, Firefox or Safari. (If you don't see the bar, show it from the View menu.)

<a href="javascript:%0A%28function%28%29%7Bif%28window.__dbe%29%7Breturn%3B%7D%0Awindow.__dbe%3Dtrue%3Bif%28document.body.childNodes.length%3D%3D%3D0%29%7Balert%28%22Due%20to%20a%20bug%20in%20Google%20Chrome%20%28issue%20%2393199%29%2C%20this%20tool%20will%20not%20work%20%22%2B%22for%20searches%20conducted%20via%20Chrome%27s%20address%20bar.%20To%20fix%20the%20issue%2C%20do%20%22%2B%22any%20of%20the%20following%3A%5Cn%5Cn%22%2B%22%2A%20Search%20from%20www.google.com%20instead%20of%20from%20the%20address%20bar.%5Cn%5Cn%22%2B%22%2A%20Go%20to%20File%20-%3E%20New%20Tab%2C%20right%20click%20on%20the%20%5C%22Google%20Search%5C%22%20Chrome%20%22%2B%22app%20and%20click%20%5C%22Remove%20from%20Chrome%5C%22.%20This%20will%20fix%20searches%20from%20the%20%22%2B%22address%20bar.%5Cn%5Cn%22%2B%22%2A%20Use%20another%20browser%2C%20such%20as%20Firefox.%22%29%3B%7D%0Avar%20anchor%3Ddocument.getElementsByTagName%28%27script%27%29%5B0%5D%3Bvar%20script%3Ddocument.createElement%28%27script%27%29%3Bscript.src%3D%27%2F%2Ffocusontheuser.org%2Fdontbeevil%2Fscript.js%3F%27%2B%28new%20Date%28%29.getTime%28%29%29%3Banchor.parentNode.insertBefore%28script%2Canchor%29%3B%7D%29%28%29%3B">don't be evil</a>

This proof of concept was built by some engineers at Facebook, Twitter and MySpace, in consultation with several other social networking companies. We are open-sourcing the code so that anyone may use it or make it even better.

Contact us at team@focusontheuser.org